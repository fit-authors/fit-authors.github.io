---
layout: default
title: Events
permalink: /events/
---
# Events

{% assign sorted = site.events | sort: 'date' | reverse %}
{% for event in sorted %}
  {% include event-slide.html %}
{% endfor %}
