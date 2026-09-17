---
layout: default
title: Blog
permalink: /blog/
---

# Blog

<ol class="blog-index">
{% for post in site.posts %}
  <li>
    <a href="{{ post.url | relative_url }}">
      <time datetime="{{ post.date | date: '%Y-%m-%d' }}">{{ post.date | date: '%-d %B, %Y' }}</time>:
      {{ post.title }}
    </a>
  </li>
{% endfor %}
</ol>
