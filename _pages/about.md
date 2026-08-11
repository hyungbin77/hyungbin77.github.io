---
permalink: /
title: "통계로 문제를 정의하고, 모델을 운영까지 가져갑니다"
excerpt: "통계학 석사 수료 · 국민연금 기금운용본부 기금정보AI팀 · 금융 데이터와 AI 모델 개발"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

전북대학교 통계학과에서 학사와 석사 과정(수료)을 마쳤고,
현재 **국민연금 기금운용본부 기금정보AI팀**에서 금융 모델과 데이터 플랫폼을 다루고 있습니다.

시계열 이상탐지, 생존분석 캘리브레이션, LLM 생성 텍스트 판별처럼
**통계적으로 검증 가능한 형태로 문제를 좁히는 일**을 주로 해왔습니다.
분석에서 끝내지 않고 모델이 실제로 돌아가는 환경까지 맡는 쪽에 관심이 있습니다.

**관심 직무** — 데이터 사이언티스트 / ML 엔지니어 / AI 서비스 개발

## 기술 스택

| 구분 | 내용 |
| --- | --- |
| 분석 · 통계 | Python, R, SPSS |
| 데이터베이스 | Oracle SQL |
| 백엔드 · 애플리케이션 | Java, Spring, Nexacro |
| 인프라 | Kubernetes, Linux |

## 주요 이력

- **국민연금 기금운용본부 기금정보AI팀** (2026.01 ~ 현재) — 금리변동요인모델·Enhanced Index 전략모델 개발 및 운용, EDM 및 빅데이터 포털 운영, LLM 모델 관리
- **NeurIPS 2025** — *KSP: Kolmogorov-Smirnov metric-based Post-Hoc Calibration for Survival Analysis* 공동저자
- **응용통계연구** — AI 생성 텍스트 판별 연구 제1저자 (심사 중)
- **한국기계산업진흥회** — 무역 시계열 데이터 기반 이상탐지 모형 검토 연구 1·2차 수행

{% assign featured = site.portfolio | sort: 'date' | reverse %}
{% if featured.size > 0 %}
프로젝트 상세는 [프로젝트]({{ '/projects/' | relative_url }}), 논문은 [연구]({{ '/research/' | relative_url }}),
전체 이력은 [이력서]({{ '/resume/' | relative_url }}) 페이지에 정리해 두었습니다.
{% endif %}

## 연락

- 이메일 — [{{ site.author.email }}](mailto:{{ site.author.email }})
- GitHub — [github.com/{{ site.author.github }}](https://github.com/{{ site.author.github }})
