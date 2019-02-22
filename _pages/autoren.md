---
layout: page
title: Normen
permalink: /normen/
---
<ul>
  {% for item in site.data.sammlung %}

      <li><a href="{{ item.url }}">{{ item.title }}</a></li>

  {% endfor %}
</ul>
