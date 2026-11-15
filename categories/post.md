---
layout: default
title: "POST"
permalink: /categories/post/
---

# POST

<ul>
{% for post in site.categories.POST %}
  <li>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <small> — {{ post.date | date: "%Y-%m-%d" }}</small>
  </li>
{% endfor %}
</ul>
