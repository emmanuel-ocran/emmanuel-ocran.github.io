---
layout: single
title: ""
author_profile: true
classes: wide
---

&nbsp;  


Hi! I'm **Ocran** — an associate data scientist and analyst.

I help businesses and nonprofits make smarter decisions by transforming complex data into clear, actionable insights.

With a background in finance and growing expertise in cloud analytics, I design scalable solutions that simplify reporting, uncover trends, and drive measurable impact.

<div style="margin-top: 1rem;">
  <a href="https://drive.google.com/file/d/1DUUEciicVQzL8aN42of_AV_uRFBhouDO/view?usp=sharing"
     class="btn btn--primary"
     target="_blank" rel="noopener">
     View My Resume
  </a>
  <a href="/about"
     class="btn btn--secondary"
     style="margin-left: 15px;"
     target="_blank" rel="noopener">
     Learn More About Me
  </a>
</div>

&nbsp;
---

## What I Do

- Data analysis and visualization using Python, SQL, Excel, and Power BI  
- Cloud-based data workflows and reporting with AWS (S3, Athena, Lambda)  
- Business-focused analytics in finance, operations, and education domains  
- Interactive dashboards and performance reports for smarter decisions  

---

## Latest Projects

<div class="entries-grid" style="display: grid; grid-template-columns: 1fr 1fr; gap: 1.5rem;">

  {% assign latest_projects = site.projects | sort: 'date' | reverse %}
  {% for project in latest_projects limit:2 %}
    <div class="project-card" style="border: 1px solid #ddd; padding: 1rem; border-radius: 8px; background: #fff;">
      {% if project.image %}
        <img src="{{ project.image | relative_url }}" alt="{{ project.title }}" style="width: 100%; height: auto; border-radius: 6px; margin-bottom: 0.5rem;" />
      {% endif %}
      <h3 style="margin-top: 0;">
        <a href="{{ project.link }}" target="_blank">{{ project.title }}</a>
      </h3>
      <p style="font-size: 0.9rem; color: #666;"><strong>{{ project.date | date: "%B %d, %Y" }}</strong></p>
      <p style="font-size: 0.95rem;">{{ project.description | truncate: 140 }}</p>
      <a href="{{ project.link }}" target="_blank" style="font-size: 0.9rem;">View project →</a>
    </div>
  {% endfor %}

</div>


---


## Recent Posts

<div class="entries-grid" style="display: grid; grid-template-columns: 1fr 1fr 1fr; gap: 1.5rem;">

  {% for post in site.posts limit:3 %}
  <div class="post-card" style="border: 1px solid #ddd; border-radius: 8px; padding: 1rem;">
    {% if post.header.image %}
    <img src="{{ post.header.image | relative_url }}" alt="{{ post.title }}" style="width: 100%; height: auto; border-radius: 6px; margin-bottom: 0.5rem;" />
    {% endif %}
    <h4 style="margin-top: 0;">
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    </h4>
    <p style="font-size: 0.85rem; color: #666;">{{ post.date | date: "%B %d, %Y" }}</p>
    <p style="font-size: 0.9rem;">{{ post.excerpt | truncate: 120 }}</p>
    <a href="{{ post.url | relative_url }}" style="font-size: 0.85rem;">Read more →</a>
  </div>
  {% endfor %}

</div>

