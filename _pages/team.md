---
title: "InfiniAI Lab - Team"
layout: team
excerpt: "InfiniAI Lab: Team members"
sitemap: false
permalink: /people/
---

<p class="team-recruiting"><i class="fas fa-bullhorn"></i> We are looking for new PhD students, Postdocs, and Master students to join the team! <a href="{{ site.baseurl }}/vacancies">See openings →</a></p>

## Faculty

<div class="team-grid">
{% for member in site.data.team_members limit:1 %}
<div class="member-card member-card-pi">
<img src="{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="member-photo member-photo-pi" />
<div class="member-info">
<h4 class="member-name">{{ member.name }}</h4>
<span class="member-role member-role-pi">{{ member.info }}</span>
<span class="member-email"><i class="fas fa-envelope"></i> {{ member.email }}</span>
</div>
</div>
{% endfor %}
</div>

## PhD Students & Postdocs

<div class="team-grid">
{% for member in site.data.team_members offset:1 %}
{% unless member.info contains "Master" %}
<div class="member-card">
<img src="{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="member-photo" />
<div class="member-info">
<h4 class="member-name">{{ member.name }}</h4>
<span class="member-role">{{ member.info }}</span>
<span class="member-email"><i class="fas fa-envelope"></i> {{ member.email }}</span>
</div>
</div>
{% endunless %}
{% endfor %}
</div>

## Master Students

<div class="team-grid">
{% for member in site.data.team_members offset:1 %}
{% if member.info contains "Master" %}
<div class="member-card">
<img src="{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="member-photo" />
<div class="member-info">
<h4 class="member-name">{{ member.name }}</h4>
<span class="member-role">{{ member.info }}</span>
<span class="member-email"><i class="fas fa-envelope"></i> {{ member.email }}</span>
</div>
</div>
{% endif %}
{% endfor %}
</div>

## Alumni

<div class="alumni-grid">
{% for member in site.data.alumni_members %}
<div class="alumni-card">
<div class="alumni-name">{{ member.name }}</div>
<div class="alumni-info">{{ member.info }}</div>
</div>
{% endfor %}
</div>

<div class="alumni-section-extra">
<h4>Visitors and Undergraduate Students</h4>
<div class="alumni-grid">
<div class="alumni-card">
<div class="alumni-name">Haoyun Chen</div>
<div class="alumni-info">Undergrad → PhD at Princeton University</div>
</div>
<div class="alumni-card">
<div class="alumni-name">Jingwei Zuo</div>
<div class="alumni-info">MS → PhD at Rice University</div>
</div>
<div class="alumni-card">
<div class="alumni-name">Chen Li</div>
<div class="alumni-info">MS → PhD at CMU</div>
</div>
<div class="alumni-card">
<div class="alumni-name">Yiying Luo</div>
<div class="alumni-info">MS → PhD at CMU</div>
</div>
<div class="alumni-card">
<div class="alumni-name">Wentao Guo</div>
<div class="alumni-info">MS → PhD at Princeton University</div>
</div>
</div>
</div>
