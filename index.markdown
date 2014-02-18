---
layout: default
---

My name is Nick Mango and I own some [companies](/about), collect some [records](http://nick.limitedpressing.com), and write some [articles](/articles).

### Recent Articles

<ul>
  {% for post in site.posts limit:10 %}
    <li><a href="{% if post.permalink %}{{ post.permalink }}{% else %}{{ post.url }}{% endif %}">{{ post.title }}</a> on {{ post.date | date: "%b %d, %Y" }}</li>
  {% endfor %}
</ul>

See a list of all my articles [here](/articles), or find out more about me [here](/about).