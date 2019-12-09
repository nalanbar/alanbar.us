---
title: Aviation 
subtitle: all posts tagged "aviation"
layout: layouts/base.njk
---
## Post pages

<h1>Tagged “{{ aviation }}”</h1>

<ol>
{% set taglist = collections[ tag ] %}
{% for post in taglist | reverse %}
  <li><a href="{{ post.url | url }}">{{ post.data.title }}</a></li>
{% endfor %}
</ol>
