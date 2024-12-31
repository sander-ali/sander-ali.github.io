---
layout: page
title: "Program Design"
year: 2024
semester: "Fall"
department: "Computer Science"
level: "UnderGraduate"
credits: 3
description: "2024_Program_Design."
permalink: /teaching/program-design/
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


2024_Program_Design