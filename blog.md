---
layout: blog
title: Blob
permalink: /blog/
---
<h3>Posts</h3>
<ul>
  {% for post in site.posts %}
  <li>
    <a href="http://arghh.github.io/Hello-World/">{{ post.title }}</a>
  </li>
  {% endfor %}
</ul>
