---
layout: page
title: Course Calendar
nav_order: 2
description: An embedded Google Calendar displaying the weekly event schedule.
---

# Course Calendar

{% for module in site.modules %}
{{ module }}
{% endfor %}

---
