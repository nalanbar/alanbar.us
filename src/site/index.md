---
title: Alanbar Aviation 
subtitle: The musings of an idiot, who dreamed of flying.<br> <small>Managed by <a href="https://twitter.com/nabilalanbar">Nabil</a></small>.
layout: layouts/base.njk
---
### This site is a training log.

That bears repeating: this site is meant to be a training log. I am still learning how to fly. I am not a CFI. I am not YOUR CFI. Shit, I can't even fly without someone else in the right seat. Assume anything I write about flight is incorrect. Technology is another matter altogether. Assume I have that locked down tight. 

I intend to use it to document my struggles and triumphs as I get my pilots license, but I may also post other things from time to time. To that end, I've included a menu item at the top for my aviation posts. Everything else will have to be found in my post collection. 

## Post pages

<ul class="listing">
{%- for page in collections.post | reverse -%}

<li>
    <a href="{{ page.url }}">{{ page.data.title }}</a> -
    <time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLLL d, y") }}</time>
  </li>
{%- endfor -%}
</ul>
