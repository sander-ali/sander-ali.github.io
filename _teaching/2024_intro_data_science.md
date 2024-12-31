---
layout: page
title: "Python for Data Management"
year: 2024
semester: "Spring"
department: "Computer Science"
level: "Graduate"
credits: 3
description: "2024_python_for_data_management."
permalink: /teaching/python-for-data-management/
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


2024_python_for_data_management