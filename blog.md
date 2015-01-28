---
layout: blog
title: Blob
permalink: /blog/
---

## All posts
  {% for post in site.posts %}
  <li>
    <a href="http://arghh.github.io">{{ post.title }}</a>
  </li>
  {% endfor %}
