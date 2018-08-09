---
title: Apereo Events
permalink: events/
---

<img class="apereo-hero" src="{{ "/assets/image/undraw/undraw_events_2p66.svg" | absolute_url }}" alt="events" />

# Events

<ul class="mdl-list">

{% for item in site.events %}

  <li class="mdl-list__item mdl-list__item--two-line">
    <a href="{{ item.url }}">
      <i class="material-icons">calendar_today</i>
      <span>{{ item.title }}</span>
      <span class="mdl-list__item-sub-title">{{ item.description }}</span>
    </a>
  </li>

{% endfor %}

</ul>
