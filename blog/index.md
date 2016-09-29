---
layout: page
title: My blog posts over the years
excerpt: "An archive of blog posts sorted by date."
image:
  feature: 600x200.png
  credit: Josh Atwell
  creditlink: https://twitter.com/josh_atwell
search_omit: true
---

Hang loose... it's all coming back soon. Keep in mind these have been through a WordPress, OctoPress, GitHub Pages, and themes blender at this point so forgive any formatting issues.

<ul class="post-list">
{% for post in site.categories.blog %} 
  <li><article><a href="{{ site.url }}{{ post.url }}">{{ post.title }} <span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span>{% if post.excerpt %} <span class="excerpt">{{ post.excerpt | remove: '\[ ... \]' | remove: '\( ... \)' | markdownify | strip_html | strip_newlines | escape_once }}</span>{% endif %}</a></article></li>
{% endfor %}
</ul>
