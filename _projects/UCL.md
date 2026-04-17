---
title: UCL
layout: default
description: "Collection of resources created whilst at UCL"
permalink: /ucl
---

# UCL Resources 
Here are a collection of resources I created (with the help of others) while at University College, London from 2023-2026.

{% for project in site.ucl %}
### [{{ project.title }}]({{ project.url | relative_url }})

{{ project.description }}

{% endfor %}