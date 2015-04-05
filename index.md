---
layout: home
permalink: /
title: "Carlos Meza"
excerpt: "DevOps Ninja Guru and Unicorn"
image:
  feature: banner-front.svg
---
This site is dedicated to the awesomeness that is [Carlos Meza](https://www.linkedin.com/in/cmeza99). Here you can find out more about him and see what he has been up to. This site, much like me, will forever be a work in progress.

<div class="tiles">

<div class="tile">
  <h2 class="post-title"><a href="/archive/" title="Post archive">Timeline</a></h2>
  <p class="post-excerpt">This is an archive of my posts. You can see my experiences and follow my adventures.</p>
</div><!-- /.tile -->

<div class="tile">
  <h2 class="post-title">Portfolio</h2>
  <p class="post-excerpt">Being built</p>
</div><!-- /.tile -->

<div class="tile">
  <h2 class="post-title"><a href="/likes/" title="Things I like">Inspirations</a></h2>
  <p class="post-excerpt">Things I like and inspire me.</p>
</div><!-- /.tiles -->

<div class="tile">
  <h2 class="post-title"><a href="/about/" title="About Carlos Meza">About Me</a></h2>
  <p class="post-excerpt">Just a brief bio and history of yours truly.</p>
</div><!-- /.tile -->

</div><!-- /.tile -->

<div style="clear:both"></div>

## Recent Posts

<div class="tiles">
{% for post in site.posts %}
	{% include post-list.html %}
{% endfor %}
</div><!-- /.tiles -->

