---
title: "InfiniAI Lab - Blog"
layout: publications
excerpt: "InfiniAI Lab -- Blog."
sitemap: false
permalink: /blog/
---

<div class="blog-header" markdown="0">
<h1><i class="fas fa-flask"></i> Research Highlights</h1>
</div>

{% for publi in site.data.publist %}
{% if publi.highlight == 1 %}
<div class="blog-entry" markdown="0">
<h3 class="blog-title"><a href="{{ publi.link.blog }}">{{ publi.title }}</a></h3>
<p class="blog-authors"><i class="fas fa-users"></i> {{ publi.authors }}</p>
<p class="blog-desc">{{ publi.description }}</p>
<div class="blog-links">
<a href="{{ publi.link.blog }}" class="blog-btn blog-btn-primary"><i class="fas fa-book-open"></i> Read More</a>
<a href="{{ publi.link.url }}" class="blog-btn blog-btn-outline"><i class="fas fa-file-alt"></i> Paper</a>
</div>
</div>
{% endif %}
{% endfor %}
