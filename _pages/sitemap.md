---
layout: archive
title: "사이트맵"
permalink: /sitemap/
author_profile: true
---

{% include base_path %}

이 사이트의 모든 페이지 목록입니다. 검색엔진용 [XML 버전]({{ base_path }}/sitemap.xml)도 있습니다.

<h2>페이지</h2>
{% for post in site.pages %}
  {% include archive-single.html %}
{% endfor %}

<h2>프로젝트</h2>
{% for post in site.portfolio %}
  {% include archive-single.html %}
{% endfor %}

<h2>연구</h2>
{% for post in site.publications %}
  {% include archive-single.html %}
{% endfor %}

<h2>기록</h2>
{% for post in site.posts %}
  {% include archive-single.html %}
{% endfor %}
