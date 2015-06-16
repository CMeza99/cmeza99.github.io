---
layout: home
permalink: /
title: "Root"
excerpt: "DevOps Ninja Guru and Unicorn"
image:
  feature: banner-front.jpg
modified: 2015-06-15T28:22:00-07:00
post_count: 8
---

&nbsp;

<div class="tiles">

<div class="tile"></div>

<div class="tile">
  <div class="center">{% include images/documents.svg %}</div>
  <h2 class="center" style="margin:auto"><a href="/archive/" title="Post archive">Changelog</a></h2>
</div><!-- /.tile -->

<!--
<div class="tile">
  <h2 class="post-title">Portfolio</h2>
  <p class="post-excerpt">Being built</p>
</div><!-- /.tile -->
<!--
<div class="tile">
  <h2 class="post-title"><a href="/likes/" title="Things I like">Inspirations</a></h2>
  <p class="post-excerpt">Things that inspire and motivate me. Hopefully, this can give another perspective to my personality.</p>
</div><!-- /.tile -->

<div class="tile">
  <div class="center">{% include images/user.svg %}</div>
  <h2 class="center" style="margin:auto"><a href="/about/" title="About Carlos Meza">About Me</a></h2>
</div><!-- /.tile -->

<div class="title"></div>

</div><!-- /.tile -->

<div style="clear:both"></div>

## Recent Posts
{% assign count=page.post_count %}
<div class="tiles">
{% for post in site.posts %}
	{% if count > 0 %}
	 {% include post-grid.html %}
	 {% assign count=count | minus:1 %}
	{% endif %}
{% endfor %}
</div><!-- /.tiles -->
<div style="text-align:center">
  <a href="/archive/" class="btn">Older Posts</a>
</div><!-- /.tile -->
