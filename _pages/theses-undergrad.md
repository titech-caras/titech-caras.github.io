---
title: 卒業論文
layout: text
permalink: /theses-undergrad.html
---

## 卒業論文
{% for thesis in site.data.theses-undergrad %}
  {% if thesis.hr %}<hr>
  {% else %}<ul style="list-style-type: none"><li>
  <b>{{ thesis.title }}</b>
  <em>{{ thesis.name }}</em>（{{ thesis.info }}）
  </li></ul>{% endif %}
{% endfor %}
