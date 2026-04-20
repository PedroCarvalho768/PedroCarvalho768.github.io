---
layout: home
title: Blog
---

{% for post in site.posts %}
  <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
  <p class="meta">{{ post.date | date: "%B %d, %Y" }}</p>
  <div class="content">
    {{ post.content }}
  </div>
  <hr>
{% endfor %}
