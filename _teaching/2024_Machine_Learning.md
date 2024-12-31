---
layout: page
title: "Machine Learning"
year: 2024
semester: "Fall"
department: "Computer Science"
level: "WorkDay Employees"
credits: 3
description: "2024_Machine_Learning."
permalink: /teaching/Machine-Learning/
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


2024_Machine_Learning