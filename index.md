---
layout: home
permalink: /
title: "All About Carlos"
excerpt: "DevOps Ninja Guru and Unicorn"
image:
  feature: banner-front.svg
---

<div class="tiles">
{% for post in site.posts %}
	{% include post-grid.html %}
{% endfor %}
</div><!-- /.tiles -->
