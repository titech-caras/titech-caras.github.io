---
title: ニュース
layout: text
permalink: /news.html
---

# ニュース
{% for article in site.data.news %}
<p>{{ article.date }} <br>
<em>{{ article.headline }}</em>
{% if article.content %}<br>{{ article.content }}{% endif %}</p>
{% endfor %}
