---
layout: page
permalink: /
description: "A food blog about a hipster living in Nashville."
tags: [hungry hipster,review, food, blog, nashville, restaurant, what, to, eat, drink,]
---

<ul class="post-list">
{% for post in site.posts limit:3 %} 
  <li><article><a href="{{ site.url }}{{ post.url }}">{{ post.title }} <span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span></a></article></li>
{% endfor %}
</ul>