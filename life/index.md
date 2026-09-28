---
layout: page
title: Life
description: Personal reflections by Tharcisse
permalink: /life/
---

A space for personal reflections and stories along the way.

<ul>
  {% for post in site.categories.life %}
  {% if post.type == "post" %}
    <li>
        <span>{{ post.date | date_to_string }}</span> » <a href="{{ post.url | relative_url }}" title="{{ post.title }}">{{ post.title }}</a>
        <meta name="description" content="{{ post.summary | escape }}">
        <meta name="keywords" content="{{ post.tags | join: ', ' | escape }}"/>
    </li>
  {% endif %}
  {% endfor %}
</ul>
