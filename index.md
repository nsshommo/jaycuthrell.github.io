---
layout: page
title: "Jay Cuthrell"
image:
  feature: 1year.jpg
  credit: Jay Cuthrell
  creditlink: https://jaycuthrell.com
---

### Speaker Bio

![My Gravatar](https://www.gravatar.com/avatar/377cdaacd95f70842298d3b0d0713c8c.jpg?s=200)

Jay Cuthrell is Chief of Staff to the SVP & Chief Technology Officer of [Dell EMC Converged Platforms & Solutions](http://vce.com). He is a frequent industry speaker currently based in the United States. Previously, as a strategic technology consultant with <a href="http://cuthrell.com">cuthrell.com</a> he worked with service providers, startup companies, and investment groups in addition to writing for ReadWrite and Telecompetitor. He has held CTO, VP, and GM roles at Digitel and NeoNova as well as infrastructure consulting roles working domestically and internationally for Fortune 500 clients while at Scient and iXL. He also served at Nortel, AIC, IBM, and North Carolina State University College of Engineering. He holds a BS in Materials Science and Engineering from North Carolina State University and grew up in Beaufort, NC. His blog can be found at <a href="https://jaycuthrell.com">jaycuthrell.com</a>

### Business Card

![My current Dell EMC business card](/images/dell-emc-business-card.png)

### Honorarium

An honorarium in the form of an anonymous charitable donation to a bona fide charitable group is encouraged but not required (quid pro quo).

### Disclosure

Please read my [disclosure](https://jaycuthrell.com/disclosure/).

### Blog Posts: 1998 to Present

These posts have been through a series of imports and exports. Originally, flat files, then they became WordPress (LAMP), OctoPress (LAMP), GitHub Pages, Revue (imported), etc... not to mention the various themes blender at this point. So, please forgive any formatting issues.

<ul class="post-list">
{% for post in site.categories.blog %}
  <li><article><a href="{{ site.url }}{{ post.url }}">{{ post.title }} <span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span>{% if post.excerpt %} <span class="excerpt">{{ post.excerpt | remove: '\[ ... \]' | remove: '\( ... \)' | markdownify | strip_html | strip_newlines | escape_once }}</span>{% endif %}</a></article></li>
{% endfor %}
</ul>
