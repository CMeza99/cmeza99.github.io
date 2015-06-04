---
layout: home
permalink: /
title: "Root"
excerpt: "DevOps Ninja Guru and Unicorn"
image:
  feature: banner-front.jpg
modified: 2015-06-03T22:00:00-07:00
post_count: 8
---
I am Carlos Meza. I do systems administration, web development, study information security, and on occasion play with electronics.

This is where I introduce myself to the Internet. Here I share my experiences around my technical adventurers, information systems and anything nerdy. If anything here sounds interesting and you would like more information please contact me at contact@carlosmeza.com.

<div class="tiles">

<div class="tile">
  <h2 class="post-title"><a href="/archive/" title="Post archive">Timeline</a></h2>
  <p class="post-excerpt">Here is an archive of my posts in chronological order. You can see my experiences and follow my adventures.</p>
</div><!-- /.tile -->

<div class="tile">
  <h2 class="post-title">Portfolio</h2>
  <p class="post-excerpt">Being built</p>
</div><!-- /.tile -->

<div class="tile">
  <h2 class="post-title"><a href="/likes/" title="Things I like">Inspirations</a></h2>
  <p class="post-excerpt">Things that inspire and motivate me. Hopefully, this can give another perspective to my personality.</p>
</div><!-- /.tile -->

<div class="tile">
  <h2 class="post-title"><a href="/about/" title="About Carlos Meza">About Me</a></h2>
  <p class="post-excerpt">Just a brief bio and history of yours truly.</p>
</div><!-- /.tile -->

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
