---
layout: page
title: "Jay Cuthrell"
image:
  feature: 1year.jpg
  credit: Jay Cuthrell
  creditlink: https://jaycuthrell.com
---

### Business Card

![My current Dell EMC business card](/images/dell-emc-business-card.png)

### Disclosure

Please read my [disclosure](https://jaycuthrell.com/disclosure/).

### Blog Posts: 1998 to Present

These posts have been through a series of imports and exports. Originally, flat files, then they became WordPress (LAMP), OctoPress (LAMP), GitHub Pages, Revue (imported), etc... not to mention the various themes blender at this point. So, please forgive any formatting issues.

<ul class="post-list">
{% for post in site.categories.blog %}
  <li><article><a href="{{ site.url }}{{ post.url }}">{{ post.title }} <span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span>{% if post.excerpt %} <span class="excerpt">{{ post.excerpt | remove: '\[ ... \]' | remove: '\( ... \)' | markdownify | strip_html | strip_newlines | escape_once }}</span>{% endif %}</a></article></li>
{% endfor %}
</ul>
