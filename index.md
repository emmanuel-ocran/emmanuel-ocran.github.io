---
layout: single
title: ""
author_profile: true
---

&nbsp;  
&nbsp;

Hi! I'm **Ocran** — an associate data scientist and analyst.

I help businesses and nonprofits make smarter decisions by transforming complex data into clear, actionable insights.

With a background in finance and growing expertise in cloud analytics, I design scalable solutions that simplify reporting, uncover trends, and drive measurable impact.

<div style="margin-top: 1rem;">
  <a href="https://drive.google.com/file/d/1DUUEciicVQzL8aN42of_AV_uRFBhouDO/view?usp=sharing" class="btn btn--primary">View My Resume</a>
  <a href="/about" class="btn btn--light-outline" style="margin-left: 10px;">Learn More About Me</a>
</div>

&nbsp;  
&nbsp;

---

## What I Do

- Data analysis and visualization using Python, SQL, Excel, and Power BI  
- Cloud-based data workflows and reporting with AWS (S3, Athena, Lambda)  
- Business-focused analytics in finance, operations, and education domains  
- Interactive dashboards and performance reports for smarter decisions  

---

## Latest Projects

{% for project in site.projects limit:2 %}
<div style="margin-bottom: 2rem;">

  {% if project.image %}
  <img src="{{ project.image | relative_url }}" alt="{{ project.title }}" style="width:100%; max-width: 600px; border-radius: 8px; margin-bottom: 0.75rem;" />
  {% endif %}

  ### [{{ project.title }}]({{ project.link }})
  <small><strong>{{ project.date | date: "%B %d, %Y" }}</strong></small>

  {{ project.description }}

  <br>
  <a href="{{ project.link }}" class="btn btn--light-outline">View Project</a>
</div>

---
{% endfor %}


## Recent Posts

{% for post in site.posts limit:3 %}
### [{{ post.title }}]({{ post.url | relative_url }})
<small><strong>{{ post.date | date: "%B %d, %Y" }}</strong> — {{ post.reading_time }} read</small>

{{ post.excerpt }}

[Read more]({{ post.url | relative_url }})  
---
{% endfor %}
