---
title: メンバー
layout: grid
permalink: /people
---

### 教員
{% assign number_printed = 0 %}
{% for member in site.data.staff %}

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

### 博士課程
{% assign number_printed = 0 %}
{% for member in site.data.students-phd %}

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

### 修士課程
{% assign number_printed = 0 %}
{% for member in site.data.students-master %}

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

### 学士課程
{% assign number_printed = 0 %}
{% for member in site.data.students-undergrad %}

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

---

### 卒業生
#### <a href="theses-master">修士課程</a>
{% for member in site.data.alumni-master %}

<div style="text-indent:1em">
  {% if member.website %}
  <h5><a href="{{ member.website }}">{{ member.name }}</a>（{{ member.info }}）</h5>
  {% else %}
  <h5>{{ member.name }}（{{ member.info }}）</h5>
  {% endif %}
</div>

{% endfor %}

#### <a href="theses-undergrad">学士課程</a>
{% for member in site.data.alumni-undergrad %}

<div style="text-indent:1em">
  {% if member.website %}
  <h5><a href="{{ member.website }}">{{ member.name }}</a>（{{ member.info }}）</h5>
  {% else %}
  <h5>{{ member.name }}（{{ member.info }}）</h5>
  {% endif %}
</div>

{% endfor %}
