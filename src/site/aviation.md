---
title: IamNabil Aviation 
subtitle: The musings of an idiot, who dreamed of flying.<br /> Managed by <a href="https://twitter.com/nabilalanbar">Nabil</a>.
layout: layouts/base.njk
---
## This site is a training log.

This site is meant to be a training log. I intend to use it to document my struggles and triumphs as I get my pilots license.

## Post pages

<h1>Tagged “{{ aviation }}”</h1>

<ol>
{% set taglist = collections[ tag ] %}
{% for post in taglist | reverse %}
  <li><a href="{{ post.url | url }}">{{ post.data.title }}</a></li>
{% endfor %}
</ol>
