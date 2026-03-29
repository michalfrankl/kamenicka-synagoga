---
layout: page
title: Novinky
permalink: /novinky/
---

  {% for post in site.posts %}
    {%- assign date_format = site.minima.date_format | default: "%-d. %-m. %Y" -%}

      <div><span class="post-meta">{{ post.date | date: date_format }}</span></div> <div><a href="{{ post.url | relative_url }}">{{ post.title }}</a></div>

  {% endfor %}


