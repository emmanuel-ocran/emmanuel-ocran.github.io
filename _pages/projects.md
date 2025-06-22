---
title: "Projects"
permalink: /projects/
layout: single
author_profile: true
---

Explore practical projects showcasing my work in data analytics, cloud and web development.

<div class="entries-grid" style="display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 1.5rem;">

{% assign sorted_projects = site.projects | sort: 'date' | reverse %}
{% for project in sorted_projects %}
  <div class="project-card" style="border: 1px solid #ddd; border-radius: 8px; padding: 1rem; background-color: #fff;">
    {% if project.image %}
      <img src="{{ project.image | relative_url }}" alt="{{ project.title }}" style="width: 100%; height: 180px; object-fit: cover; border-radius: 6px; margin-bottom: 0.75rem;" />
    {% endif %}
    <h3 style="margin-top: 0;">
      <a href="{{ project.link }}" target="_blank" style="text-decoration: none;">{{ project.title }}</a>
    </h3>
    <p style="font-size: 0.85rem; color: #666;">{{ project.date | date: "%B %d, %Y" }}</p>
    <p>{{ project.description }}</p>
    <a href="{{ project.link }}" target="_blank" style="font-size: 0.85rem; color: #007ACC;">View project →</a>
  </div>
{% endfor %}

</div>
