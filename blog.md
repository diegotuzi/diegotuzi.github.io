---
layout: default
title: Blog
---

# Latest Posts

Welcome to my Blog. In this section you can find several resources. There are projects related to my academic and work path, my thesis works and other posts. I hope you enjoy reading my posts. I'll be happy to receive any feedback. 

---
{% for tag in site.tags %}
  <h3>{{ tag[0] }}</h3>
  <ul>
    {% for post in tag[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}