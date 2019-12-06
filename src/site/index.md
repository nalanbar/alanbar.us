---
title: IamNabil Aero 
subtitle: .The musings of an idiot, who dreamed of flying.<br /> Managed by <a href="https://twitter.com/nabilalanbar">Nabil</a>.
layout: layouts/base.njk
---


## This site is a starting point

This site is meant to capture my aviation career, even though it is not a career, and I don't actually fly. Yet. 

## Post pages

The pages found in in the posts

<ul class="listing">
{%- for page in collections.post -%}
  <li>
    <a href="{{ page.url }}">{{ page.data.title }}</a> -
    <time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLLL d, y") }}</time>
  </li>
{%- endfor -%}
</ul>
