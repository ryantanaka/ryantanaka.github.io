---
layout: page
title: Projects
permalink: /projects/
---

# hi this is a projects page

{% for project in site.projects %}

<img src="{{site.baseurl}}/assets/img/{{project.icon}}">

# {{ project.title }}
{{ project.content }}


***

{% endfor %}
