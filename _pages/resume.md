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

**Data Scientist** — Time Series · NLP
모델이 내놓은 숫자를 그대로 믿지 않습니다. 예측이 얼마나 신뢰할 수 있는지를 검증 가능한 형태로 만드는 일을 해왔습니다.

## 학력
* **전북대학교 통계학과 석사 수료**, 2024.09 ~ 2026.08
  * 지도교수 김광수 · 학점 3.88
* **전북대학교 통계학과 학사 졸업**, 2017.03 ~ 2024.08
  * 학점 3.54

## 경력
* **AIDA ROOT** — 국민연금 기금운용본부 기금정보AI팀 파견, 2026.01 ~ 현재
  * 금융 예측모델 검증 및 운영 — 금리변동요인모델, Enhanced Index 전략모델
  * EDM(Enterprise Data Management) 운영 — 리서치 골든카피 데이터 정합성 관리
  * 빅데이터 포털 운영 — 리서치 · 시장 데이터 제공
  * 업무 활용 LLM 모델 관리

## 기술 스택
* **Languages** — Python, R, SQL (Oracle), Java, SPSS
* **ML / DL** — PyTorch, TensorFlow, scikit-learn, pandas, numpy
* **Statistics** — 생존분석, 시계열 분석, 이상탐지, 회귀분석, 변화점 탐지
* **NLP / LLM** — LDA, 문체 분석, Perplexity, LLM API, RAG, 파인튜닝, NLTK, gensim
* **Framework** — Spring, Nexacro (유지보수 및 기능 개발)
* **Environment** — Linux, Kubernetes (배포 · 운영)
* **Tools** — Git

## 연구 실적
{% assign research = site.publications | sort: 'date' | reverse %}
{% if research.size > 0 %}
  <ul>{% for post in research %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
{% else %}
  <p><em><code>_publications/</code> 에 항목을 추가하면 이 목록이 자동으로 채워집니다.</em></p>
{% endif %}

## 프로젝트 · 수행과제
{% assign projects = site.portfolio | sort: 'date' | reverse %}
{% if projects.size > 0 %}
  <ul>{% for post in projects %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
{% else %}
  <p><em><code>_portfolio/</code> 에 프로젝트를 추가하면 이 목록이 자동으로 채워집니다.</em></p>
{% endif %}

## 교육 · 조교 · 멘토링
* **SPSS 강의 조교**, 전북대학교 — 2024 겨울학기, 2025 여름학기
  * 통계 분석 실습 강의 조교로 2개 학기 참여, 수강생 실습 지도
* **머신러닝 교과목 신규 개발 조교**, 빅데이터 혁신융합대학 사업단 — 2024.07 ~ 2024.12
  * 한 학기 분량 강의 콘텐츠와 PPT 전체 제작. 강의에서 다루는 모델 수만큼 실습 코드(Python, R) 개발
  * 강의 영상 최종 검수 — 오탈자 확인 및 대학 요구 양식에 맞춘 편집
* **학부생 멘토링**, 전북대학교 튜터링 동아리 — 2025.07 ~ 2025.08
  * 통계학과 학부생 2명 대상 주 1회 스터디 주도. 선형대수, Linux 서버 사용법 교육
  * 회귀분석 증명 과정과 커널(Kernel) 개념은 강의 자료를 직접 제작하여 설명

## 자격 · 어학
* **OPIc** — Intermediate High (IH), 2026.08 응시
