---
title: Portfolio
layout: page
---

{% raw %}
<div class="project-list">
  {% for project in site.projects %}
    <div class="project-card">
      <h3>
        <a href="{{ project.url }}">{{ project.title }}</a>
      </h3>

      <p>{{ project.description }}</p>

      <p>
        <strong>Tech:</strong> {{ project.tech | join: ", " }}
      </p>
    </div>
  {% endfor %}
</div>
{% endraw %}
