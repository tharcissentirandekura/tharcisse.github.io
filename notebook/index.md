---
layout: page
title: Notebook
description: Notes by Tharcisse
permalink: /notebook/
---

A place to collect what I learn, useful references, and notes to return to.

<ul>
  {% for post in site.categories.notebook %}
    <li>
        <span>{{ post.date | date_to_string }}</span> » {% if post.highlight %}&starf; {% endif %}<a href="{{ post.url | relative_url }}" title="{{ post.title }}">{{ post.title | truncate:72 }}</a>
    </li>
  {% endfor %}
</ul>
