---
title: Publications
layout: base-en
permalink: /publications-en
---

## 2019
{% for pub in site.data.publications-2019 %}
  {% if pub.language == "English" %}
  <ul><li><b>{{ pub.title }}</b><br />
  <em>{{ pub.authors }}</em><br />
  {{ pub.venue }}, {{ pub.year }}. (acceptance rate: {{ pub.rate }} )<br />
  {% if pub.award %}<font class="award"><b>{{ pub.award }}</b></font><br />{% endif %}
  {% endif %}
{% endfor %}
