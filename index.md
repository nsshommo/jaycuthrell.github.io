---
layout: page
title: "Jay Cuthrell"
image:
  feature: 600x200.png
---
### Contact Information

<blockquote class="twitter-tweet" lang="en"><p lang="en" dir="ltr">My new <a href="https://twitter.com/VCE">@VCE</a> business cards arrived <a href="http://t.co/q9QATsEUBJ">pic.twitter.com/q9QATsEUBJ</a></p>&mdash; Jay Cuthrell (@JayCuthrell) <a href="https://twitter.com/JayCuthrell/status/627899573449535492">August 2, 2015</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

### Speaker Bio

Jay Cuthrell is a Director within the Global Office of the Chief Technology Officer (OCTO) for the Converged Platforms and Solutions Division of [Dell EMC](http://www.vce.com). He is a frequent industry speaker currently based in the United States. Previously, as a strategic technology consultant with <a href="http://cuthrell.com">cuthrell.com</a> he worked with service providers, startup companies, and investment groups in addition to writing for ReadWrite and Telecompetitor. He has held CTO, VP, and GM roles at Digitel and NeoNova (formerly an Azure Capital and Bridgescale Partners portfolio company now a NRTC Company) and infrastructure consulting roles working domestically and internationally for Fortune 500 clients. He also served at Scient (formerly iXL now Publicis), Nortel, Analysts International, IBM, and NCSU College of Engineering. He holds a BS in Materials Science and Engineering from North Carolina State University and grew up in Beaufort, NC. His blog can be found at <a href="http://jaycuthrell.com">jaycuthrell.com</a>

### Honorarium 

An honorarium in the form of an anonymous charitable donation to a bona fide charitable group is encouraged but not required (quid pro quo).

### Resum&eacute;

Please read my [professional summary](http://jaycuthrell.com/resume/).

### Disclosure

Please read my [disclosure](http://jaycuthrell.com/disclosure/).

### Recent Blog Posts


<ul class="post-list">
{% for post in site.posts limit:10 %}
  <li><article><a href="{{ site.url }}{{ post.url }}">{{ post.title }} <span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span>{% if post.excerpt %} <span class="excerpt">{{ post.excerpt | remove: '\[ ... \]' | remove: '\( ... \)' | markdownify | strip_html | strip_newlines | escape_once }}</span>{% endif %}</a></article></li>
{% endfor %}
</ul>
