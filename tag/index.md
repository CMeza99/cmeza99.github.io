---
title: Tags
layout: default
description: Tag list
permalink: /tag/
---

{% assign tags_list = site.tags %}

<h2 class='tag-header'>Tags</h2>
<ul>
  {% if tags_list.first[0] == null %}
	{% for tag in tags_list %}
	  <li>
		<a href="/tag/{{ tag | slugify }}" class='list-group-item'>{{ tag | capitalize }}</a>
		<span class='badge'>{{ site.tags[tag].size }}</span>
	  </li>
	{% endfor %}
  {% else %}
	{% for tag in tags_list %}
	  <li>
		<a href="/tag/{{ tag[0] | slugify }}" class='list-group-item'>{{ tag[0] | capitalize }}</a>
		<span class='badge'>{{ tag[1].size }}</span>
	  </li>
	{% endfor %}
  {% endif %}
</ul>
{% assign tags_list = nil %}
