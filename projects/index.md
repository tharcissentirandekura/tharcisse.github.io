---
layout: page
title: Projects
description: Projects by Tharcisse
permalink: /projects/
---

A home for my projects and work in progress. You can also explore my [public repositories on GitHub](https://github.com/tharcissentirandekura?tab=repositories).

<ul>
  {% for post in site.categories.projects %}
    <li>
        <span>{{ post.date | date_to_string }}</span> » <a href="{{ post.url | relative_url }}" title="{{ post.title }}">{{ post.title }}</a>
        <meta name="description" content="{{ post.summary | escape }}">
        <meta name="keywords" content="{{ post.tags | join: ', ' | escape }}"/>
    </li>
  {% endfor %}
</ul>
