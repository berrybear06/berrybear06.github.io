---
layout: default
title: The Berries
description: My engineering and programming projects!
---

# Projects

{% for project in site.projects %}
### {% if project.ext-link %} [{{ project.name }}]({{ project.ext-link }}) {% else %} {{ project.name }} {% endif %}
{% if project.img-link %}
![{{ project.name }}]({{ site.url | append: project.img-link }} "{{ project.name }}")
{% endif %}
{{ project.content | markdownify }}
{% endfor %}