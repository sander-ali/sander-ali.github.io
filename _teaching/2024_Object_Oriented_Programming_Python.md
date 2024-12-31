---
layout: page
title: "Object Oriented Programming (Python)"
year: 2024
semester: "Fall"
department: "Computer Science"
level: "UnderGraduate"
credits: 3
description: "2024_Object_oriented_programming_python."
permalink: /teaching/object-oriented-programming-python/
---



## {{ page.title }} ({{ page.year }}, {{ page.semester }})
- **Department:** {{ page.department }}
- **Level:** {{ page.level }}
- **Credits:** {{ page.credits }}
- **Description:** {{ page.description }}
- **Materials:**
  {% for material in page.materials %}
  - {{ material | markdownify }}
  {% endfor %}


2024_Object_oriented_programming_python