---
title: Apereo Projects
layout: default
permalink: projects/
---

## Projects

<ul class="mdl-list">

{% for project in site.projects %}
  {% if project.incubation != true %}

    <li class="mdl-list__item mdl-list__item--two-line">
      <a href="{{ project.url }}">
        <i class="material-icons mdl-list__item-avatar">public</i>
        <span>{{ project.title }}</span>
        <span class="mdl-list__item-sub-title">{{ project.description }}</span>
      </a>
    </li>

  {% endif %}
{% endfor %}

</ul>

## Incubation Projects


<ul class="mdl-list">

{% for project in site.projects %}
  {% if project.incubation == true %}

    <li class="mdl-list__item mdl-list__item--two-line">
      <a href="{{ project.url }}">
        <i class="material-icons mdl-list__item-avatar">public</i>
        <span>{{ project.title }}</span>
        <span class="mdl-list__item-sub-title">{{ project.description }}</span>
      </a>
    </li>

  {% endif %}
{% endfor %}

</ul>
