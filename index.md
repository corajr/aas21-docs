---
layout: page
title: AAS21 Documentation
exclude_from_search: true
---
Instructions for site maintenance of AAS21.

{% for category in site.categories %} 
  <h2 id="{{ category[0] }}-ref">{{ category[0] | join: "/" | capitalize }}</h2>
  <ul>
    {% assign pages_list = category[1] %}  
    {% include JB/pages_list %}
  </ul>
{% endfor %}
