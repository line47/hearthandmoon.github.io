---
layout: default
title: Elixrs
permalink: /elixrs/
---

<ul class="projects">
{% assign sorted = site.elixrs | sort: 'sortOrder' %}
 {% for elixrs in sorted %}
  <li class="project-item">
    <a href="{{ elixrs.url }}" class="project-name">
      <img src="{{ elixrs.smallImage }}"/>
      {{ elixrs.title }}
    </a>
    <p>{{ elixrs.shortDescription }}</p>
  </li>
{% endfor %}
</ul>
