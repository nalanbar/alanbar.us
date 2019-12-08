---
layout: layouts/base.njk
pageClass: posts
templateEngineOverride: njk, md
---

<p class="date">
  Posted by an Alanbar on <time datetime="{{ date }}">{{ date | dateDisplay }}</time>
</p>
<main>
  {{ content | safe }}
  <div class="footnote"; font-size: 0.7em;>
    <p>
      This page is part of the posts section.
    </p>
  </div>
</main>
