---
title: People
layout: grid-en
permalink: /people-en
---

## Staff
{% assign number_printed = 0 %}
{% for member in site.data.staff-en %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/files/images/people/{{ member.photo }}" class="img-responsive" width="30%" style="float: left" /><br />
  {% if member.website %}
  <h4><a href="{{ member.website }}">{{ member.name }}</a></h4>
  {% else %}
  <h4>{{ member.name }}</h4>
  {% endif %}
  {{ member.info }}<br>
  <a href="mailto:{{ member.email }}">{{ member.email }}</a>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}