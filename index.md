---
weight: 0
layout: default
title: John Taylor Gatto Archive
---

<ol class="rectangle-list">
  {% assign pageList = site.pages | sort: 'weight' %}
  {% for p in pageList %}
    {% if p.path contains 'en-US' and p.title != page.title %}
      <li>
        <a {% if p.url == page.url %}class="active"{% endif %} href="{{ p.url }}">
          {{ p.title }}
        </a>
      </li>
    {% endif %}
  {% endfor %}
</ol>

