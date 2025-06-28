---
title: "Projects"
permalink: /projects/
layout: single
author_profile: true
---

Explore practical, hands-on projects showcasing my work in data analytics, cloud, and web development.

<ul class="project-list" style="list-style: none; padding: 0; margin-top: 2rem;">
  {% assign sorted_projects = site.projects | sort: 'date' | reverse %}
  {% for project in sorted_projects %}
    <li style="margin-bottom: 2rem; padding-bottom: 1.5rem; border-bottom: 1px solid #e5e5e5;">
      <h3 style="margin-bottom: 0.25rem; font-size: 1.25rem;">
        <a href="{{ project.link }}" target="_blank" style="text-decoration: none; color: #007ACC;">{{ project.title }}</a>
      </h3>
      <p style="margin: 0; font-size: 0.85rem; color: #666;">
        {{ project.date | date: "%B %d, %Y" }}
        {% if project.skills %}
          &nbsp;|&nbsp;
          <span style="color: #888;">Skills:</span>
          <span style="color: #444;">{{ project.skills | join: ', ' }}</span>
        {% endif %}
      </p>
      <p style="margin-top: 0.75rem;">{{ project.description }}</p>
      <p>
        <a href="{{ project.link }}" target="_blank" style="font-size: 0.85rem; color: #007ACC;">View project →</a>
      </p>
    </li>
  {% endfor %}
</ul>
