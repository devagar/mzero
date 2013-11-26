---
layout: default
title: Arquivo	
---
### Artigos Publicados

<div class="hfeed">
	{% for post in site.posts %}
	   <article class="hentry entry">
	    	<p><time datetime="{{ post.date | xmlschema }}">{{ post.date | date: "%Y-%m-%d" }}</time>
	    	<a href="{{ post.url }}">{{ post.title }}</a></p>
	    </article>
	{% endfor %}
</div>
