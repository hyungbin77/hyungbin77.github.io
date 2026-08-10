---
permalink: /
title: "데이터로 문제를 정의하고, 코드로 끝까지 만듭니다"
excerpt: "통계학 석사 수료 · 데이터 분석 / 머신러닝 · IT·AI 직무 신입 지원"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

<!-- ────────────────────────────────────────────────────────────────
     채워야 할 곳은 「」 로 표시해 두었습니다. 전부 채운 뒤 이 주석은 지우세요.
     이 페이지는 채용 담당자가 30초 안에 읽는 화면입니다.
     길게 쓰지 말고, 아래 프로젝트 페이지로 넘어가게 만드는 것이 목적입니다.
     ──────────────────────────────────────────────────────────────── -->

전북대학교에서 통계학 석사 과정을 수료했습니다. 학위 과정에서는 「연구 주제 한 줄」을 다뤘고,
그 과정에서 익힌 **문제를 숫자로 정의하는 습관**과 **가설을 검증 가능한 형태로 쪼개는 방식**을
지금은 서비스와 제품을 만드는 쪽에서 쓰고 싶습니다.

연구자로 남기보다, **분석 결과가 실제로 동작하는 무언가가 되는 지점**에 관심이 있습니다.
그래서 모델을 만드는 데서 멈추지 않고 데이터 수집부터 배포까지 직접 굴려보는 프로젝트를 이어가고 있습니다.

**지원 희망 직무** — 데이터 분석 / ML 엔지니어 / AI 서비스 개발 (신입)

기술 스택
======

| 구분 | 내용 |
| --- | --- |
| 언어 | 「Python, R, SQL 등 실제로 쓸 수 있는 것만」 |
| 분석 · 통계 | 「pandas, numpy, statsmodels, 다루어 본 통계 방법론」 |
| 머신러닝 · 딥러닝 | 「scikit-learn, PyTorch 등 — 프로젝트에서 써 본 것 위주로」 |
| 데이터 · 인프라 | 「PostgreSQL, Docker, AWS 등」 |
| 협업 | 「Git, GitHub, Notion, Jira 등」 |

> 스택은 "들어본 것"이 아니라 **프로젝트에서 실제로 써 본 것**만 적는 편이 신뢰를 얻습니다.
> 각 항목이 어느 프로젝트에서 쓰였는지 아래에서 바로 확인되면 가장 좋습니다.

대표 프로젝트
======

{% assign featured = site.portfolio | sort: 'date' | reverse %}
{% if featured.size > 0 %}
<ul>
{% for item in featured limit:3 %}
  <li><strong><a href="{{ item.url }}">{{ item.title }}</a></strong>{% if item.summary %} — {{ item.summary }}{% endif %}</li>
{% endfor %}
</ul>

전체 목록은 [프로젝트]({{ '/projects/' | relative_url }}) 페이지에 있습니다.
{% else %}
아직 등록된 프로젝트가 없습니다. `_portfolio/` 에 파일을 추가하면 이 목록과
[프로젝트]({{ '/projects/' | relative_url }}) 페이지에 자동으로 나타납니다.
{% endif %}

연락
======

- 이메일 — [{{ site.author.email }}](mailto:{{ site.author.email }})
- GitHub — [github.com/{{ site.author.github }}](https://github.com/{{ site.author.github }})
- 이력서 — [한 장 요약 보기]({{ '/resume/' | relative_url }})
