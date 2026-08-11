---
title: "AI 생성 텍스트 판별 — 데이터셋 구축부터 특징 선택까지"
excerpt: "Quora 크롤링과 4종 LLM API로 데이터셋을 직접 구축하고, 문체 지표 기반으로 생성 텍스트를 판별했습니다. 제1저자 논문."
collection: portfolio
date: 2025-11-30
summary: "LLM 생성 텍스트 판별 (제1저자 논문)"
---

**기간** — 2025.11
**역할** — 제1저자 (응용통계연구 투고, 심사 중)
**기술** — Python, Lexical Density, LDA, Forward Selection

## 진행 내용

- **데이터셋 직접 구축** — Quora 질의응답 크롤링(인간 작성) + Gemini, GPT 등 4종 LLM API 응답 수집
- **문체 특징 설계** — Lexical Density, LDA 등을 판별 지표로 산출
- **특징 선택** — Forward Selection을 적용해 판별 성능을 극대화하는 특징 조합 선별

논문 정보는 [연구]({{ '/research/2025-11-01-ai-generated-text-detection/' | relative_url }}) 페이지에 있습니다.
