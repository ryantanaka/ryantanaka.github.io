---
layout: default
title: Projects
permalink: /projects/
---



{% for project in site.projects %}

  ***

  <div class="projectimage box" style="background: url({{site.baseurl}}/assets/img/{{project.icon}})"></div>

  <div class="projectinfo">
    <h1>{{ project.title }}</h1>
    {{ project.content }}
  </div>

{% endfor %}
