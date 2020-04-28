---
title: News
layout: text-en
permalink: /news-en.html
---

# News
{% for article in site.data.news-en %}
<p>{{ article.date }} <br>
<em>{{ article.headline }}</em>
{% if article.content %}<br>{{ article.content }}{% endif %}</p>
{% endfor %}
