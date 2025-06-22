---
layout: single
title: ""
author_profile: true
classes: wide
---

&nbsp;  
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

<div class="grid__wrapper">

{% assign latest_projects = site.projects | sort: 'date' | reverse %}
{% for project in latest_projects limit:2 %}
  <div class="grid__item one-half">
    <div style="border: 1px solid #ccc; padding: 1rem; border-radius: 8px;">
      {% if project.image %}
        <img src="{{ project.image }}" alt="{{ project.title }}" style="width: 100%; border-radius: 6px;" />
      {% endif %}
      <h3 style="margin-top: 0.5rem;">
        <a href="{{ project.link }}" target="_blank">{{ project.title }}</a>
      </h3>
      <p><strong>{{ project.date | date: "%B %d, %Y" }}</strong></p>
      <p>{{ project.description }}</p>
    </div>
  </div>
{% endfor %}

</div>

---


## Recent Posts

{% for post in site.posts limit:3 %}
### [{{ post.title }}]({{ post.url | relative_url }})
<small><strong>{{ post.date | date: "%B %d, %Y" }}</strong> — {{ post.reading_time }} read</small>

{{ post.excerpt }}

[Read more]({{ post.url | relative_url }})  
---
{% endfor %}
