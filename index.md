---
layout: default
title: mZero
---

<div class='post'>
    <div class='body'>{{ site.posts.first.content }}</div>
</div>
<hr>
### Artigos anteriores

<div class="hfeed">
	{% for post in site.posts %}
	   <article class="hentry entry">
	    	<p><time datetime="{{ post.date | xmlschema }}">{{ post.date | date: "%Y-%m-%d" }}</time>
	    	<a href="{{ post.url }}">{{ post.title }}</a></p>
	    </article>
	{% endfor %}
</div>
