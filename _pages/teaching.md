---
layout: page
permalink: /teaching/
title: Teaching
description: Courses and teaching activities at various institutions
nav: true
nav_order: 4
---

### Teaching Philosophy
I believe in fostering critical thinking and practical skills through hands-on learning experiences...

### Courses

{% for course in site.teaching %}
##### [{{ course.title }} ({{ course.year }}, {{ course.semester }})]({{ course.url }})
{% endfor %}
