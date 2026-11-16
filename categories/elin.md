---
layout: default
title: "Elin"
permalink: /categories/elin/
---

# Elin

<ul>
{% for post in site.categories.Elin %}
  <li>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <small> — {{ post.date | date: "%Y-%m-%d" }}</small>
  </li>
{% endfor %}
</ul>
