---
layout: homepage
title: Blog
permalink: /blog/
published: false   # blog is on hold; set to true to activate
---

## Blog

<ul class="post-list">
{% for post in site.posts %}
  <li>
    <span class="post-list-date">{{ post.date | date: "%b %-d, %Y" }}</span>
    <a class="post-list-title" href="{{ post.url | relative_url }}">{{ post.title }}</a>
    {% if post.description %}
    <div class="post-list-desc">{{ post.description }}</div>
    {% endif %}
  </li>
{% endfor %}
</ul>
