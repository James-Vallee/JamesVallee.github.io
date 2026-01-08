---
layout: default
title: Personal Projects
permalink: /personal/
nav: personal
banner_image: /assets/images/black.png
subtitle:  
---

<section class="project-grid">
  {% if site.personal.size > 0 %}
    {% for project in site.personal %}
      <a class="project-item" style="background-image: url('{{ project.image }}');"
         href="{{ project.url }}">
        <div class="overlay"></div>
        <div class="project-text">
          <h3>{{ project.title }}</h3>
        </div>
      </a>
    {% endfor %}
  {% else %}
    <div class="coming-soon">
      <p>🚧 Personal projects are coming soon! 🚧</p>
    </div>
  {% endif %}
</section>
