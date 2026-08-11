---
layout: archive
title: "이력서"
permalink: /resume/
author_profile: true
redirect_from:
  - /cv/
  - /cv.html
---

{% include base_path %}

{% if site.resume_pdf %}
<p><a href="{{ site.resume_pdf | relative_url }}" class="btn btn--inverse">PDF 이력서 다운로드</a></p>
{% endif %}

**관심 직무** — 데이터 사이언티스트 / ML 엔지니어 / AI 서비스 개발
**요약** — 통계학 석사 수료. 금융 도메인에서 모델 개발·운용과 데이터 플랫폼 운영을 함께 맡고 있습니다.

## 학력
* **전북대학교 통계학과 석사 수료**, 2024.09 ~ 2026.08
* **전북대학교 통계학과 학사 졸업**, 2017.03 ~ 2024.08

## 경력
* **AIDA ROOT** — 국민연금 기금운용본부 기금정보AI팀 파견, 2026.01 ~ 현재
  * 금융 모델 개발 및 운용 — 금리변동요인모델, Enhanced Index 전략모델
  * EDM(Enterprise Data Management) 및 빅데이터 포털 운영 — 리서치 골든카피 데이터, 시장 데이터
  * LLM 모델 관리

## 기술 스택
* **분석 · 통계** — Python, R, SPSS
* **데이터베이스** — Oracle SQL
* **백엔드 · 애플리케이션** — Java, Spring, Nexacro
* **인프라** — Kubernetes, Linux

## 프로젝트 · 수행과제
{% assign projects = site.portfolio | sort: 'date' | reverse %}
{% if projects.size > 0 %}
  <ul>{% for post in projects %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
{% else %}
  <p><em><code>_portfolio/</code> 에 프로젝트를 추가하면 이 목록이 자동으로 채워집니다.</em></p>
{% endif %}

## 연구
{% assign research = site.publications | sort: 'date' | reverse %}
{% if research.size > 0 %}
  <ul>{% for post in research %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
{% else %}
  <p><em><code>_publications/</code> 에 항목을 추가하면 이 목록이 자동으로 채워집니다.</em></p>
{% endif %}

## 교육 · 조교 · 멘토링
* **SPSS 강의 조교**, 전북대학교 — 2024 겨울학기, 2025 여름학기
* **통계학과 후배 멘토링**, 전북대학교 튜터링 동아리 — 2025.07 ~ 2025.08
  * 머신러닝 관심 학부생 2명 대상 주 1회 스터디 운영. 선형대수, 회귀분석 증명, 커널(Kernel) 개념, Linux 서버 기초 강의 자료 제작
* **'데이터 마이닝' 교과목 개발 조교**, 빅데이터 혁신융합대학 사업단 — 2024.07 ~ 2024.12
  * 강의 콘텐츠 및 실습용 R 코드 제작, 강의 영상 검수 및 편집

## 교육 이수
* **한국인공지능학회 춘계 단기강좌** — 2025.05.29 ~ 2025.05.30
  * Agentic AI 이해 및 응용. AI Agent와 Agentic AI의 구분, 다중 에이전트 협업, LLMOps 기반 업무 자동화, 자율 시스템의 안전성과 GPU 자원 활용
* **한국인공지능학회 동계 단기강좌** — 2025.02.19 ~ 2025.02.21
  * LLM의 상식 기반 추론과 인과 학습, 이미지·3D 형상 생성, 강화학습 기초, Distribution Shifts 하의 안정적 학습, Probabilistic Graphical Model

## 자격 · 어학
* **SQLD** (SQL 개발자)
* **OPIc IH**
