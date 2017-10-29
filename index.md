---
layout: page
title: "Jay Cuthrell"
image:
  feature: 1year.jpg
  credit: Jay Cuthrell
  creditlink: https://jaycuthrell.com
---

### Discussion Leader Bio

Jay Cuthrell is Chief of Staff to the SVP & Chief Technology Officer of Dell EMC Converged Platforms & Solutions. He is a frequent industry discussion leader on trending and emergent impactful technology. An innovative and sought after energetic industry leader, Jay leverages his extensive experiences as a CTO, VP, and GM in high growth ICT companies as well as global infrastructure consulting roles for Fortune 500 clients to be a trusted advisor on strategic technology.

Jay’s expertise demonstrated through strong growth and change cycles provides a unique perspective into the future of the technology industry. His previous engagements include providing a key role as a consultant through cuthrell.com, where he worked closely with service providers, startup companies, and investment groups. Jay is a published industry author in ReadWrite, Telecompetitor, and NTCA Roundtable as well as a frequent corporate blogger.

Jay holds a BS in Materials Science and Engineering from North Carolina State University and grew up in Beaufort, North Carolina. His personal blog can be found at [jaycuthrell.com](https://jaycuthrell.com/).

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
