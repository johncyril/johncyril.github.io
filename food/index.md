---
layout: page
title: Food
category: PAGE
description: Great food I'm fortunate enough to eat or flukey enough to cook. 
byline: Probably not worth your time should you dislike the idea of eating anything that once mooed, bleated or clucked.
---

<div class="home">

  <h1 class="page-heading">Recipes</h1>

  <ul class="post-list">
    {% for recipe in site.recipes reversed%}
      <li>
        <span class="post-meta">{{ recipe.date | date: "%b %-d, %Y" }}</span>
		<h2>
          <a class="post-link" href="{{ recipe.url | prepend: site.baseurl }}">{{ recipe.title }}</a>
        </h2>
		{{ recipe.excerpt }}		
		<img src="{{ site.baseurl }}{{ recipe.preview-image }}" width="300" />
        </li>
    {% endfor %}
  </ul>

  <!--<p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>-->

</div>