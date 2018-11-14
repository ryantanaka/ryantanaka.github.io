---
layout: default
title: Projects
permalink: /projects/
---

# Projects I Have Worked On

Below is a collection of some of the projects, for both academic and personal purposes, that I have
worked on and found to be meaningful.

<span class="label label-info">Languages</span>
<span class="label label-default">Frameworks/Tools</span>

{% assign projects = site.projects | sort:"order" %}
{% for project in projects %}

  ***

  <div id="projectimage-{{ forloop.index }}" class="projectimage box" style="background: url({{site.baseurl}}/assets/img/{{project.icon}})"></div>

  <div class="projectinfo">
    <h1 class="black">{{ project.title }}</h1>
    {{ project.content }}
  </div>

{% endfor %}
