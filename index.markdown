---
layout: homepage
author: john
tags: []
---

<h1> Hello </h1>

{{ site.description }}

<div>
{% for page in site.pages %}
	
	{% if page.title %}	
		<h2> <a heref="{{ page.url | prepend: site.baseurl }}"> {{ page.title }} </a> </h2>
		{{ page.description }}   		
		
	{% endif %}
	<br>

{% endfor %}
</div>