---
layout: home
permalink: /
title: "Root"
excerpt: "DevOps Ninja Guru and Unicorn"
image:
  feature: banner-front.jpg
modified: 2015-05-12T20:40:00-07:00
post_count: 8
---
<p>This site is dedicated to the awesomeness that is [Carlos Meza](https://www.linkedin.com/in/cmeza99). At the moment this site is intended to provide insight to who I am and what I do. I am sharing my interests and experience with who ever wants to know more about me. Most posts are brief, but as this site stabilizes they should become more detailed. Much like me, this site will forever be a work in progress.</p>

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


{% for post in paginator.posts %}
  <h1><a href="{{ post.url }}">{{ post.title }}</a></h1>
  <p class="author">
    <span class="date">{{ post.date }}</span>
  </p>
  <div class="content">
    {{ post.content }}
  </div>
{% endfor %}

<div class="pagination">
  {% if paginator.previous_page %}
    <a href="{{ paginator.previous_page_path }}" class="previous">Previous</a>
  {% else %}
    <span class="previous">Previous</span>
  {% endif %}
  <span class="page_number ">Page: {{ paginator.page }} of {{ paginator.total_pages }}</span>
  {% if paginator.next_page %}
    <a href="{{ paginator.next_page_path }}" class="next">Next</a>
  {% else %}
    <span class="next ">Next</span>
  {% endif %}
</div>



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

