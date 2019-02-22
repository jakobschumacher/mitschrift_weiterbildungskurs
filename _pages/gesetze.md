---
layout: page
title: Gesetzessammlung
permalink: /gesetze/
---





{% assign mydocs = site.gesetze | group_by: 'level' %}
{% for cat in mydocs %}
<h2>{{ cat.name | capitalize }}</h2>
<ul>
      {% assign items = cat.items  %}
      {% for item in items %}
<li><a href="{{ item.url }}">{{ item.title }}</a></li>
      {% endfor %}
</ul>
{% endfor %}







<h2>Infektionsschutz</h2>
{% assign groups = site.gesetze | where:'thema', "Infektionsschutz" | group_by: "thema" | sort: "name" %}
<ul>

{% for group in groups %}
    {% for item in group.items %}
    <li><a href="{{ item.iminternet }}">{{ item.name }}</a></li>
    {%endfor%}
{%endfor%}
</ul>

<h2>Trinkwasser</h2>
{% assign groups = site.gesetze | where:'thema', "Trinkwasser" | group_by: "thema" | sort: "name" %}
<ul>
{% for group in groups %}
    {% for item in group.items %}
    <li><a href="{{ item.iminternet }}">{{ item.name }}</a></li>
    {%endfor%}
{%endfor%}
</ul>
