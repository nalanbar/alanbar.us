---
title: Alanbar Aviation 
subtitle: The musings of an idiot, who dreamed of flying.<br> <small>Managed by <a href="https://twitter.com/nabilalanbar">Nabil</a></small>.
layout: layouts/base.njk
---
## This site is a training log.

This site is meant to be a training log. I intend to use it to document my struggles and triumphs as I get my pilots license.

## Post pages

<ul class="listing">
{%- for page in collections.post -%}
  <li>
    <a href="{{ page.url }}">{{ page.data.title }}</a> -
    <time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLLL d, y") }}</time>
  </li>
{%- endfor -%}
</ul>
