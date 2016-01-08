---
permalink: /archiv/
group: "navigation-04"
title: Archiv
lang: de
id: archive
description: Alle Posts auf einem Blick
---
{% if site.baseurl != '' or null %}
    {% assign base = site.baseurl %}
{% else %}
    {% assign base = '' %}
{% endif %}

{% assign posts = site.posts | where:"lang", page.lang %}

Datum | Titel | Tags
---|---|---
{% for post in posts%}{% include date.md %} | [{{ post.title }}]({{ post.url }}) | {% for tag in post.tags %} <a href="{{ site.tag_dir | prepend: base }}/{{ tag }}" class="tag">{{ tag }}</a> {% endfor %}
{% endfor %}
