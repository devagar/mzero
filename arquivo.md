---
layout: default
title: Arquivo	
---
### Artigos Publicados

<div class="hfeed">
	{% for post in site.posts %}
	   <article class="hentry entry">
	    	<p><time datetime="{{ post.date | xmlschema }}">{{ post.date | date: "%d-%m" }}</time>
	    	<a href="{{ post.url }}">{{ post.title }}</a></p>
	    </article>
	    {% if year != nyear %} 
       			 <h3 class="date_title">{{ post.date | date: '%Y' }}</h3>
 		{% endif %}
	{% endfor %}
</div>
