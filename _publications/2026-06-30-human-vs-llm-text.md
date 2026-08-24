---
title: "인간과 기계 생성 언어 비교 및 판별 방법론 연구"
collection: publications
category: journal
excerpt: "LLM이 생성한 텍스트와 사람이 쓴 텍스트를 해석 가능한 문체 지표만으로 구분한 연구. 공동 제1저자."
date: 2026-06-30
venue: '응용통계연구 (The Korean Journal of Applied Statistics) 39(3)'
paperurl: 'https://doi.org/10.5351/KJAS.2026.39.3.235'
citation: '박형빈, 강신성, 이기훈, 김광수. (2026). &quot;인간과 기계 생성 언어 비교 및 판별 방법론 연구.&quot; <i>응용통계연구</i>, 39(3), 235–255. (공동 제1저자)'
---

*Study on comparative and discriminatory methodology of human and machine-generated languages*

LLM이 생성한 텍스트와 사람이 쓴 텍스트를 **해석 가능한 문체 지표만으로** 구분할 수 있는지 검증한 연구입니다.
공동 제1저자로 데이터 구축부터 분류기 설계까지 전 과정을 담당했습니다.

## 데이터셋 자체 구축

공개 데이터셋에 의존하지 않고 비교 가능한 구조로 직접 설계했습니다.

| 출처 | 문서 수 | 토큰 수 |
| --- | --- | --- |
| Human (Quora) | 2,833 | 864,660 |
| GPT-4o | 3,000 | 950,147 |
| Gemini 2.0 Flash | 3,000 | 787,117 |
| Claude 3.7 Sonnet | 3,000 | 599,155 |
| DeepSeek | 3,000 | 679,558 |
| **합계** | **14,833** | **3,880,637** |

질문 100개를 모형별로 30회씩 반복 생성했고, 5개 주제로 층화했습니다.
프롬프트 4유형을 검토해 편향을 유발하는 유형을 제외하고 단일 공통 프롬프트를 설계했습니다.

## 특징 설계

- **문체 분석** — 고유 단어 수, 개인 대명사 비율, 어휘 밀도(lexical density), Flesch-Kincaid 가독성 지수
- **주제 분석** — LDA 주제 분포. coherence score로 주제 수를 5개로 결정하고 부주제 서브모형 구성
- **혼란도** — Llama-3.1-8B 기반 perplexity

## 분류기와 성능

은닉층 4개 DNN(256-128-64-32, batch normalization, dropout, AdamW)으로
인간 vs LLM 이진 분류와 원천 5범주 다중 분류를 동시에 수행했습니다.

| 과제 | 정확도 | F1 |
| --- | --- | --- |
| 이진 분류 (인간 vs LLM) | 0.9778 | 0.9864 |
| 다중 분류 (원천 5범주) | 0.8598 | 0.8607 (Macro) |

핵심 기여는 **혼란도 단독 사용 대비 다중 분류 오분류율을 0.3866 감소**시킨 점입니다.
제안한 특징이 혼란도가 담지 못하는 원천 식별 정보를 보유함을 실증했습니다.
