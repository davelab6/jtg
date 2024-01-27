---
weight: 0
layout: default
title: John Taylor Gatto Archive
---

<ol class="rectangle-list">
  {% assign pageList = site.pages | sort: 'weight' %}
  {% for p in pageList %}
      <li>
        <a {% if p.url == page.url %}class="active"{% endif %} href="{{ p.url }}">
          {{ p.title }}
        </a>
      </li>
  {% endfor %}
</ol>

