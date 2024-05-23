---
title: 修士論文
layout: text
permalink: /theses-master.html
---

## 修士論文
{% for thesis in site.data.theses-master %}
  {% if thesis.hr %}<hr>
  {% else %}<ul style="list-style-type: none"><li>
  <b>{{ thesis.title }}</b>
  <em>{{ thesis.name }}</em>（{{ thesis.info }}）
  </li></ul>{% endif %}
{% endfor %}
