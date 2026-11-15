# 112research

## Catetories

{% for category in site.categories %}
<h3>{{ category[0] }}</h3>
<ul>
  {% for post in category[1] %}
  <li><a href="{{ post.url | relative_url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>
{% endfor %}

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
