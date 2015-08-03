---
layout: page
title: Projects
permalink: /projects/
---
<div class="proyects">

  <header class="project-header">
    <h1 class="project-title">{{ page.title }}</h1>
    <p class="project-meta">{{ page.date | date: "%b %-d, %Y" }}{% if page.author %} • {{ page.author }}{% endif %}{% if page.meta %} • {{ page.meta }}{% endif %}</p>
  </header>

  <ul class="project-list">
      {% for project in site.projects_collection %}
        <li>
          <span class="project-meta">{{ project.date | date: "%b %-d, %Y" }}</span>

          <h2>
            <a class="project-link" href="{{ project.url | prepend: site.baseurl }}">{{ project.title }}</a>
          </h2>
        </li>
      {% endfor %}
    </ul>

</div>
