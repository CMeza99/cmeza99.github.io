---
layout: article
permalink: /
title: "Timeline"
excerpt: "The things I've done"
image:
#  feature: banner-front.svg
---

<div class="tiles">
{% for post in site.posts %}
	{% include post-grid.html %}
{% endfor %}
</div><!-- /.tiles -->
