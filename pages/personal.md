---
layout: default
title: Personal Projects
permalink: /personal/
nav: personal
---

<section class="project-grid">
  {% for project in site.personal %}
    <a class="project-item" style="background-image: url('{{ project.image }}');"
       href="{{ project.url }}">
      <div class="overlay"></div>
      <div class="project-text">
        <h3>{{ project.title }}</h3>
      </div>
    </a>
  {% endfor %}
</section>
