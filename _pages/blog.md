---
title: "InfiniAI Lab - Blog"
layout: publications
excerpt: "InfiniAI Lab -- Blog."
sitemap: false
permalink: /blog/
---

<div class="blog-header">
<h1><i class="fas fa-flask"></i> Research Highlights</h1>
</div>

{% for publi in site.data.publist %}
{% if publi.highlight == 1 %}
<div class="blog-card" markdown="0">
<div class="blog-card-img">
<img src="{{ site.baseurl }}/images/pubpic/{{ publi.image }}" alt="{{ publi.title }}" />
</div>
<div class="blog-card-body">
<h3 class="blog-card-title">{{ publi.title }}</h3>
<p class="blog-card-authors"><i class="fas fa-users"></i> {{ publi.authors }}</p>
<p class="blog-card-desc">{{ publi.description }}</p>
<div class="blog-card-links">
{% if publi.link.blog %}
<a href="{{ publi.link.blog }}" class="blog-btn blog-btn-primary"><i class="fas fa-book-open"></i> Read More</a>
{% endif %}
{% if publi.link.url %}
<a href="{{ publi.link.url }}" class="blog-btn blog-btn-outline"><i class="fas fa-file-alt"></i> Paper</a>
{% endif %}
</div>
</div>
</div>
{% endif %}
{% endfor %}
