---
layout: homepage
author: john
tags: []
---

Hello 
=====

In a concerted effort to get back into writing, I've decided to revive my old, teenage, ranty blog after a good 5 years of it being offline.  

Over time, expect to find.. 
{{ site.description }}



{% for page in site.pages %}
	
{% if page.title %}	
## [{{ page.title }}]({{ page.url | prepend: site.baseurl }})

{{ page.description }}   
{% if page.byline %}
##### {{ page.byline }} 
{% endif %}

{% endif %}


{% endfor %}

