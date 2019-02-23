---
layout: page
title: Gesetze
permalink: /gesetze/
---
{% assign net = site.data.sammlung | group_by:"topic" | sort:"name" %}

{% for type in net %}
  <h1>{{ type.name }} </h1>
  <ul>
    {% for item in type.items %}
      <li><a href="{{ item.url }}">{{ item.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}
