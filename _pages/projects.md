---
layout: single
title: "Projects"
permalink: /projects/
author_profile: true
---

Explore a selection of projects where I apply data analysis, visualization, and cloud-powered insights to solve real-world problems.

---

{% for project in site.projects %}
<div style="margin-bottom: 2rem;">

  {% if project.image %}
  <img src="{{ project.image | relative_url }}" alt="{{ project.title }}" style="width:100%; max-width: 720px; border-radius: 8px; margin-bottom: 0.75rem;" />
  {% endif %}

  ### [{{ project.title }}]({{ project.link }})
  <small><strong>{{ project.date | date: "%B %d, %Y" }}</strong></small>

  {{ project.description }}

  <br>
  <a href="{{ project.link }}" class="btn btn--primary">View Project</a>
</div>

---
{% endfor %}