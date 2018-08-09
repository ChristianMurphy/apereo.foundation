---
title: Apereo Projects
permalink: projects/
description: Apereo is made up of a series of overlapping and interlocking software, regional and thematic communities.
image: /assets/image/undraw/undraw_tabs_jf82.svg
---

<img class="apereo-hero" src="{{ "/assets/image/undraw/undraw_tabs_jf82.svg" | absolute_url }}" alt="projects" />

Apereo is made up of a series of overlapping and interlocking software, regional and thematic communities.

## Projects

<ul class="mdl-list">

{% for project in site.projects %}
{% if project.incubation != true %}

    <li class="mdl-list__item mdl-list__item--two-line">
      <a href="{{ project.url }}">
        <i class="material-icons mdl-list__item-avatar">public</i>
        <span>{{ project.title }}</span>
        <span class="mdl-list__item-text-body">{{ project.description }}</span>
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
        <span class="mdl-list__item-text-body">{{ project.description }}</span>
      </a>
    </li>

{% endif %}
{% endfor %}

</ul>
