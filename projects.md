---
layout: page
nav_order: 2
permalink: /projects
---



## Projects

{% for page in site.pages %}
  {% if page.path contains 'projects/' and page.title %}
### [{{ page.title }}]({{ page.url | relative_url }})

{{ page.description }}

  {% endif %}
{% endfor %}

**Computable Z-Jump** - Defining the computable analogue of the Z-jump for equivalence relations 
**Beginners Borel** - Beginners introduction to invariant descriptive set theory\\
**ArithHier** - Building the arithmetic hierarchy for LEAN's Mathlib