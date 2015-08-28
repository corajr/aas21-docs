---
layout: page
title: AAS21 Documentation
---
Instructions for site maintenance of AAS21.

## Categories

{% for category in site.categories %} 
  <h3 id="{{ category[0] }}-ref">{{ category[0] | join: "/" | capitalize }}</h3>
  <ul>
    {% assign pages_list = category[1] %}  
    {% include JB/pages_list %}
  </ul>
{% endfor %}
