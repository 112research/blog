# 112research

## Categories

<ul>
{% for category in site.categories %}
  {% assign slug = category[0] | slugify %}
  <li><a href="{{ '/categories/' | append: slug | append: '/' | relative_url }}">{{ category[0] }}</a> ({{ category[1].size }})</li>
{% endfor %}
</ul>

## Articles

{% if site.posts.size == 0 %}
No Articles
{% else %}
<ul>
{% for post in site.posts %}
  <li>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <small> — {{ post.date | date: "%Y-%m-%d" }}</small>
  </li>
{% endfor %}
</ul>
{% endif %}
