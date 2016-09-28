---
layout: page
title: Blog
excerpt: "An archive of blog posts sorted by date."
search_omit: true
---

Hang loose... it's all coming back soon. Keep in mind these have been through a WordPress, OctoPress, GitHub Pages, and themes blender at this point so forgive any formatting issues.

{% for post in site.posts  %}
    {% capture this_year %}{{ post.date | date: "%Y" }}{% endcapture %}
    {% capture this_month %}{{ post.date | date: "%B" }}{% endcapture %}
    {% capture next_year %}{{ post.previous.date | date: "%Y" }}{% endcapture %}
    {% capture next_month %}{{ post.previous.date | date: "%B" }}{% endcapture %}

    {% if forloop.first %}
    <h2 id="{{ this_year }}-ref">{{this_year}}</h2>
    <h3 id="{{ this_year }}-{{ this_month }}-ref">{{ this_month }} {{this_year}}</h3>
    {% endif %}

    <ul class="post-list"><li><a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a> -- {% if post.date != null %} {{ post.date  | date: "%B %-d %Y" }} {% endif %} </li></ul>

    {% if forloop.last %}
    {% else %}
        {% if this_year != next_year %}
        <h2 id="{{ next_year }}-ref">{{next_year}}</h2>
        <h3 id="{{ next_year }}-{{ next_month }}-ref">{{ next_month }} {{next_year}}</h3>
        {% else %}    
            {% if this_month != next_month %}
            <h3 id="{{ this_year }}-{{ next_month }}-ref">{{ next_month }} {{this_year}}</h3>
            {% endif %}
        {% endif %}
    {% endif %}
{% endfor %}
