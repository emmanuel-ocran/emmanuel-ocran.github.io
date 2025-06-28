---
title: "Projects"
permalink: /projects/
layout: single
author_profile: true
---

Explore practical, hands-on projects showcasing my work in data analytics, cloud, and web development.

<ul class="project-cards" style="list-style: none; padding: 0; margin: 0; display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 2rem;">

  {% assign sorted_projects = site.projects | sort: 'date' | reverse %}
  {% for project in sorted_projects %}
  <li style="border: 1px solid #e0e0e0; border-radius: 12px; overflow: hidden; background-color: #fff; box-shadow: 0 2px 6px rgba(0,0,0,0.05); display: flex; flex-direction: column; height: 100%; transition: transform 0.2s ease;">
    {% if project.image %}
    <div style="width: 100%; overflow: hidden;">
      <img src="{{ project.image | relative_url }}" alt="{{ project.title }}" style="width: 100%; height: 180px; object-fit: cover;" />
    </div>
    {% endif %}

    <div style="padding: 1rem; flex-grow: 1; display: flex; flex-direction: column;">
      <h3 style="margin: 0 0 0.5rem;">
        <a href="{{ project.link }}" target="_blank" style="color: #007ACC; text-decoration: none;">{{ project.title }}</a>
      </h3>

      <p style="font-size: 0.9rem; color: #555;">{{ project.description | truncatewords: 25 }}</p>

      <p style="margin-top: auto;">
        <a href="{{ project.link }}" target="_blank" style="display: inline-block; margin-top: 1rem; font-size: 0.85rem; color: #007ACC;">View project →</a>
      </p>
    </div>
  </li>
  {% endfor %}

</ul>
