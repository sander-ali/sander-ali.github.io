---
layout: page
title: "Systems and Network Database Administration"
year: 2024
semester: "Spring"
department: "Computer Science"
level: "UnderGraduate"
credits: 3
description: "2024_Systems_Database_Administration."
permalink: /teaching/systems-database-administration/
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


2024_Systems_Database_Administration