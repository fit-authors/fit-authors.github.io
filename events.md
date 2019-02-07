---
layout: default
title: Events
---
<h1 class="text-center mb-4">{{page.title}}</h1>
{% assign sorted = site.events | sort: 'date' | reverse %}
{% for event in sorted %}
  {% include event-slide.html %}
{% endfor %}
