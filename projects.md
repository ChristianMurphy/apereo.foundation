---
title: Apereo Projects
layout: default
permalink: projects/
---

<ul class="mdl-list">

{% for item in site.projects %}

  <li class="mdl-list__item mdl-list__item--two-line">
    <a href="{{ item.url }}">
      <i class="material-icons mdl-list__item-avatar">public</i>
      <span>{{ item.title }}</span>
      <span class="mdl-list__item-sub-title">{{ item.description }}</span>
    </a>
  </li>

{% endfor %}

</ul>
