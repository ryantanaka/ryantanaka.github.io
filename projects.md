---
layout: default
title: Projects
permalink: /projects/
---

{% assign projects = site.projects | sort:"order" %}
{% for project in projects %}

  ***

  <div id="projectimage-{{ forloop.index }}" class="projectimage box" style="background: url({{site.baseurl}}/assets/img/{{project.icon}})"></div>

  <div class="projectinfo">
    <h1 class="black">{{ project.title }}</h1>
    {{ project.content }}
  </div>

{% endfor %}
