---
layout: page
nav_order: 2
permalink: /projects
---



## Projects


{% for project in site.projects %}
### [{{ project.title }}]({{ project.url | relative_url }})

{{ project.description }}

{% endfor %}

