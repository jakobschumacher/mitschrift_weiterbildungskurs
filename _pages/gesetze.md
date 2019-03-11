---
layout: blank
title: Gesetze
permalink: /gesetze/
---
{% assign gesetze = site.data.sammlung | group_by:"topic" | sort:"name" %}
<div style=" column-count: 2;">
{% for type in gesetze %}
  <h3>{{ type.name | slice: 3,50 }} </h3>
  <ul>

    {% for item in type.items %}
      <li><a href="{{ item.iminternet }}">{{ item.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}
</div>
