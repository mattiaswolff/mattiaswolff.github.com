---
layout: index
title: Blogg
tagline:
---
{% include JB/setup %}

<div class="posts">
  {% for post in site.posts %}
  <div class="post">
	<div>
		<h2><a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a> <small>({{ post.date | date_to_string }})</small></h2>
		{{ post.content }}
	</div>
	<a href="{{ BASE_PATH }}{{ post.url }}">Kommentera &raquo;</a>
	</div>
  {% endfor %}
</div>