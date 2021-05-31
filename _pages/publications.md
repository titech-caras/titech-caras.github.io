---
title: 発表論文
layout: base
permalink: /publications
---

## 2021 年
{% for pub in site.data.publications-2021 %}
  <ul><li><b>{{ pub.title }}</b><br />
  <em>{{ pub.authors }}</em><br />
  {{ pub.venue }}, {{ pub.year }}. {% if pub.rate %}(acceptance rate: {{ pub.rate }}){% endif %}<br />
  {% if pub.award %}<font class="award"><b>{{ pub.award }}</b></font><br />{% endif %}
  </li></ul>
{% endfor %}

## 2019 年
{% for pub in site.data.publications-2019 %}
  <ul><li><b>{{ pub.title }}</b><br />
  <em>{{ pub.authors }}</em><br />
  {{ pub.venue }}, {{ pub.year }}. {% if pub.rate %}(acceptance rate: {{ pub.rate }}){% endif %}<br />
  {% if pub.award %}<font class="award"><b>{{ pub.award }}</b></font><br />{% endif %}
  </li></ul>
{% endfor %}
