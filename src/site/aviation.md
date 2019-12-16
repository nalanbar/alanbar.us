---
title: Aviation 
subtitle: all posts tagged "aviation", from newest to oldest
layout: layouts/base.njk
---

<ol>
{% set taglist = collections.aviation %}
{% for post in taglist | reverse %}
  <li><a href="{{ post.url | url }}">{{ post.data.title }}</a><br><p style="margin-left: 40px"> on {{ post.data.date | dateDisplay }} </p></li>
{% endfor %}
</ol>
