---
layout: default
title: The Berries
description: My engineering and programming projects! Some of the project names are links to more info.
---

# Projects

{% assign projects = site.projects | sort: "project-order" | reverse %}
{% for project in projects %}
### {% if project.ext-link %} [{{ project.name }}]({{ project.ext-link }}) {% else %} {{ project.name }} {% endif %}
{% if project.img-link %}
![{{ project.name }}]({{ site.url | append: project.img-link }} "{{ project.name }}")
{% endif %}
{{ project.content | markdownify }}
{% endfor %}