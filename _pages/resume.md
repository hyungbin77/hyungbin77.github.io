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

<!-- ────────────────────────────────────────────────────────────────
     「」 안을 실제 이력으로 바꾸고, 해당 없는 항목은 섹션째로 지우세요.
     빈 섹션이 남아 있는 것이 없는 것보다 나쁩니다.

     PDF 이력서를 걸려면: files/ 에 PDF를 올리고
     _config.yml 의 resume_pdf 값에 경로를 적으면 아래 버튼이 나타납니다.
     ──────────────────────────────────────────────────────────────── -->

{% if site.resume_pdf %}
<p><a href="{{ site.resume_pdf | relative_url }}" class="btn btn--inverse">PDF 이력서 다운로드</a></p>
{% endif %}

**지원 직무** — 데이터 분석 / ML 엔지니어 / AI 서비스 개발 (신입)
**한 줄 요약** — 「통계 기반으로 문제를 정의하고, 모델을 서비스로 만드는 데까지 관심이 있는 신입」

학력
======
* 전북대학교 대학원 「학과명」 석사 **수료**, 「20XX. XX ~ 20XX. XX」
  * 지도교수: 「성명」 / 연구 분야: 「분야」
  * 학위 논문: 「제목」 (해당 없으면 이 줄 삭제)
* 「학부 학교명」 「전공」 학사, 「20XX. XX 졸업」
  * 학점: 「X.XX / 4.5」 (강점일 때만 적으세요)

<!-- '수료'와 '졸업'은 채용 서류에서 구분해서 봅니다.
     학위 취득 예정이면 "석사 졸업 예정 (20XX. XX)" 으로 정확히 적으세요. -->

기술 스택
======
* **언어** — 「Python, R, SQL」
* **분석 · 통계** — 「pandas, numpy, statsmodels / 회귀·시계열·베이지안 등 실제 적용해 본 방법론」
* **머신러닝 · 딥러닝** — 「scikit-learn, PyTorch / 다루어 본 문제 유형」
* **데이터 · 인프라** — 「PostgreSQL, Docker, AWS」
* **협업** — 「Git, GitHub, Notion」

경력 · 인턴 · 교육
======
* 「20XX. XX ~ 20XX. XX」 — 「기관 / 회사명」, 「역할」
  * 「담당 업무와 결과를 숫자로 한 줄」
* 「20XX. XX ~ 20XX. XX」 — 「부트캠프 / 교육과정명」
  * 「수료 내용, 최종 프로젝트」

<!-- 연구실 조교, 학부 연구생, 교내 프로젝트도 여기에 적을 수 있습니다.
     '경계 어딘가'를 보여주는 데 가장 효과적인 섹션입니다. -->

프로젝트
======
{% assign projects = site.portfolio | sort: 'date' | reverse %}
{% if projects.size > 0 %}
  <ul>{% for post in projects %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
{% else %}
  <p><em><code>_portfolio/</code> 에 프로젝트를 추가하면 이 목록이 자동으로 채워집니다.</em></p>
{% endif %}

연구 · 학회 발표
======
{% assign research = site.publications | sort: 'date' | reverse %}
{% if research.size > 0 %}
  <ul>{% for post in research %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
{% else %}
  <p><em><code>_publications/</code> 에 항목을 추가하면 이 목록이 자동으로 채워집니다.</em></p>
{% endif %}

자격증 · 어학 · 수상
======
* 「자격증명」, 「발급기관」, 「취득 연월」
* 「어학 시험명 점수」, 「응시 연월」
* 「수상명」, 「주최」, 「연월」

<!-- 데이터 직무에서 자주 보는 것: ADsP/ADP, SQLD, 빅데이터분석기사, 정보처리기사 -->
