---
layout: default
title: The Berries
description: My engineering and programming projects!
---

# Projects

{% for project in site.projects %}
- ### [{{ project.name }}]({{ project.ext-link }})
	{{ project.content | markdownify }}
{% endfor %}