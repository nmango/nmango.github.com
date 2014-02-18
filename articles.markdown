---
layout: default
permalink: articles/index.html
---

My name is Nick Mango and I own some [companies](/about), collect some [records](http://nick.limitedpressing.com), and write some [articles](/articles).

<ul>
  {% for post in site.posts %}
    <li><a href="{% if post.permalink %}{{ post.permalink }}{% else %}{{ post.url }}{% endif %}">{{ post.title }}</a> on {{ post.date | date: "%b %d, %Y" }}</li>
  {% endfor %}
</ul>