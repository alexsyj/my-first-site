---
title: Projects
layout: page
---

{% raw %}
<ul class="project-list">
  {% for project in site.projects %}
    <li>
      <h3>
        <a href="{{ project.url }}">{{ project.title }}</a>
      </h3>
      <p>{{ project.description }}</p>
      <p><strong>Tech:</strong> {{ project.tech | join: ", " }}</p>
    </li>
  {% endfor %}
</ul>
{% endraw %}
