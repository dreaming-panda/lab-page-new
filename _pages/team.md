---
title: "InfiniAI Lab - Team"
layout: gridlay
excerpt: "InfiniAI Lab: Team members"
sitemap: false
permalink: /people/
---

# Group Members

 **We are  looking for new PhD students, Postdocs, and Master students to join the team** [(see openings)]({{ site.baseurl }}/vacancies) **!**

{% assign number_printed = 0 %}
{% for member in site.data.team_members %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }} <br>email: <{{ member.email }}></i>
  <ul style="overflow: hidden">
  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> {{ member.education1 | markdownify}} </li>
  <li> {{ member.education2 | markdownify}} </li>
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

  {% if member.number_educ == 5 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  <li> {{ member.education5 }} </li>
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

# Alumni

<div class="alumni-grid" markdown="0">
<div class="alumni-card">
<span class="alumni-name">Hanshi Sun</span>
<span class="alumni-role">MS</span>
<span class="alumni-next"><i class="fas fa-arrow-right"></i> Bytedance</span>
</div>
<div class="alumni-card">
<span class="alumni-name">Jian Chen</span>
<span class="alumni-role">MS</span>
<span class="alumni-next"><i class="fas fa-arrow-right"></i> PhD at UCSD</span>
</div>
<div class="alumni-card">
<span class="alumni-name">Haoyun Qin</span>
<span class="alumni-role">Undergrad</span>
<span class="alumni-next"><i class="fas fa-arrow-right"></i> PhD at Princeton University</span>
</div>
<div class="alumni-card">
<span class="alumni-name">Jingwei Zuo</span>
<span class="alumni-role">MS</span>
<span class="alumni-next"><i class="fas fa-arrow-right"></i> PhD at Rice University</span>
</div>
<div class="alumni-card">
<span class="alumni-name">Vashisth Tiwari</span>
<span class="alumni-role">MS</span>
<span class="alumni-next"><i class="fas fa-arrow-right"></i> PhD at CMU</span>
</div>
<div class="alumni-card">
<span class="alumni-name">Chen Li</span>
<span class="alumni-role">MS</span>
<span class="alumni-next"><i class="fas fa-arrow-right"></i> PhD at CMU</span>
</div>
<div class="alumni-card">
<span class="alumni-name">Yiying Luo</span>
<span class="alumni-role">MS</span>
<span class="alumni-next"><i class="fas fa-arrow-right"></i> PhD at CMU</span>
</div>
<div class="alumni-card">
<span class="alumni-name">Wentao Guo</span>
<span class="alumni-role">MS</span>
<span class="alumni-next"><i class="fas fa-arrow-right"></i> PhD at Princeton University</span>
</div>
</div>


