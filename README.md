# blog

##Articles

{% if site.posts.size == 0 %}
まだ記事がありません。
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
