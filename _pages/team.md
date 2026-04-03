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

<div class="alumni-container">
<table class="alumni-table">
<thead>
<tr><th>Name</th><th>Role</th><th>Next Step</th></tr>
</thead>
<tbody>
<tr><td>Hanshi Sun</td><td>MS</td><td>Bytedance</td></tr>
<tr><td>Jian Chen</td><td>MS</td><td>PhD at UCSD</td></tr>
<tr><td>Haoyun Qin</td><td>Undergrad</td><td>PhD at Princeton University</td></tr>
<tr><td>Jingwei Zuo</td><td>MS</td><td>PhD at Rice University</td></tr>
<tr><td>Vashisth Tiwari</td><td>MS</td><td>PhD at CMU</td></tr>
<tr><td>Chen Li</td><td>MS</td><td>PhD at CMU</td></tr>
<tr><td>Yiying Luo</td><td>MS</td><td>PhD at CMU</td></tr>
<tr><td>Wentao Guo</td><td>MS</td><td>PhD at Princeton University</td></tr>
</tbody>
</table>
</div>


