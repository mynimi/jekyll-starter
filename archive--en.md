---
group: "navigation-04"
title: Archive
lang: en
id: archive
permalink: /en/archive/
description: An overview over every post
---
{% if site.baseurl != '' or null %}
    {% assign base = site.baseurl %}
{% else %}
    {% assign base = '' %}
{% endif %}

{% assign posts = site.posts | where:"lang", page.lang %}
Date | Title | Tags
---|---|---
{% for post in posts%}{% include date.md %} | [{{ post.title }}]({{ post.url }}) | {% for tag in post.tags %} <a href="{{ base }}/en{{ site.tag_dir }}/{{ tag }}" class="tag">{{ tag }}</a> {% endfor %}
{% endfor %}
