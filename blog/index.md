---
layout: page
title: Select blog posts
excerpt: "An archive of blog posts sorted by date."
image:
  feature: convergedthoughts.png
  credit: Jay Cuthrell
  creditlink: https://jaycuthrell.com
search_omit: true
---

These posts have been through a series of imports and exports. Originally, flat files, then they became WordPress (LAMP), OctoPress (LAMP), GitHub Pages, Revue (imported), etc... not to mention the various themes blender at this point. So, please forgive any formatting issues.

<ul class="post-list">
{% for post in site.categories.blog %}
  <li><article><a href="{{ site.url }}{{ post.url }}">{{ post.title }} <span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span>{% if post.excerpt %} <span class="excerpt">{{ post.excerpt | remove: '\[ ... \]' | remove: '\( ... \)' | markdownify | strip_html | strip_newlines | escape_once }}</span>{% endif %}</a></article></li>
{% endfor %}
</ul>
