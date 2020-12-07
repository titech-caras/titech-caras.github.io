---
title: People
layout: grid-en
permalink: /people-en
---

### Staff
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

### Students
{% assign number_printed = 0 %}
{% for member in site.data.students-grad-en %}

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
  <ul style="overflow: hidden">

  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  {% endif %}

  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}

  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %}

  </ul>
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

{% assign number_printed = 0 %}
{% for member in site.data.students-undergrad-en %}

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
  <ul style="overflow: hidden">

  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  {% endif %}

  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}

  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %}

  </ul>
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
