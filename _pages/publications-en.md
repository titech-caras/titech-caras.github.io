---
title: Publications
layout: base-en
permalink: /publications-en
---

### 2025
{% for pub in site.data.publications-2025 %}
  {% if pub.language == "English" %}
  <ul style="list-style-type: none"><li>
  <b>{{ pub.title }}</b><br />
  <em>{{ pub.authors }}</em><br />
  {{ pub.venue }}, {{ pub.year }}. {% if pub.rate %}(acceptance rate: {{ pub.rate }}){% endif %}<br />
  {% if pub.award %}<font class="award"><b>{{ pub.award }}</b></font><br />{% endif %}
  </li></ul>
  {% endif %}
{% endfor %}

### 2021
{% for pub in site.data.publications-2021 %}
  {% if pub.language == "English" %}
  <ul style="list-style-type: none"><li>
  <b>{{ pub.title }}</b><br />
  <em>{{ pub.authors }}</em><br />
  {{ pub.venue }}, {{ pub.year }}. {% if pub.rate %}(acceptance rate: {{ pub.rate }}){% endif %}<br />
  {% if pub.award %}<font class="award"><b>{{ pub.award }}</b></font><br />{% endif %}
  </li></ul>
  {% endif %}
{% endfor %}

### 2019
{% for pub in site.data.publications-2019 %}
  {% if pub.language == "English" %}
  <ul style="list-style-type: none"><li>
  <b>{{ pub.title }}</b><br />
  <em>{{ pub.authors }}</em><br />
  {{ pub.venue }}, {{ pub.year }}. {% if pub.rate %}(acceptance rate: {{ pub.rate }}){% endif %}<br />
  {% if pub.award %}<font class="award"><b>{{ pub.award }}</b></font><br />{% endif %}
  </li></ul>
  {% endif %}
{% endfor %}
