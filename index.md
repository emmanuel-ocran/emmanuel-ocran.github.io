---
layout: single
title: ""
author_profile: true
classes: wide
---

<!-- Hero Section -->
&nbsp;

Hi, I'm **Ocran** — a data scientist and analyst with a foundation in finance and a focus on scalable, cloud-based analytics.

I help organizations turn raw data into insights that drive smarter decisions, better performance, and measurable business value.

With expertise in Python, SQL, AWS, and BI tools, I build solutions that simplify reporting, uncover patterns, and power data-driven strategies across finance, education, and development sectors.

<div style="margin-top: 1rem;">
  <a href="https://drive.google.com/file/d/1DUUEciicVQzL8aN42of_AV_uRFBhouDO/view?usp=sharing"
     class="btn btn--primary"
     target="_blank" rel="noopener">View My Resume</a>

  <a href="/about" 
     class="btn" 
     style="margin-left: 15px; color: #6f777d; border: 1px solid #6f777d; padding: 0.4rem 1rem; border-radius: 5px; text-decoration: none;">Learn More About Me</a>
</div>

&nbsp;

## What I Do

<div style="display: flex; flex-wrap: wrap; gap: 1.5rem; justify-content: space-between; margin-top: 1rem;">

  <div class="service-card">
    <div class="service-icon-wrapper">
      <i class="fas fa-chart-line"></i>
    </div>
    <h4 class="service-title">Data Analysis & Visualization</h4>
    <p>Analyze, clean, and visualize data using Python, SQL, Excel, and Power BI to uncover business insights.</p>
  </div>

  <div class="service-card">
    <div class="service-icon-wrapper">
      <i class="fas fa-cloud"></i>
    </div>
    <h4 class="service-title">Cloud Data Workflows</h4>
    <p>Build automated pipelines with AWS (S3, Athena, Lambda) for scalable, cloud-native data reporting.</p>
  </div>

  <div class="service-card">
    <div class="service-icon-wrapper">
      <i class="fas fa-briefcase"></i>
    </div>
    <h4 class="service-title">Business-Focused Analytics</h4>
    <p>Deliver end-to-end analytics solutions aligned with goals in finance, education, and development sectors.</p>
  </div>

  <div class="service-card">
    <div class="service-icon-wrapper">
      <i class="fas fa-tachometer-alt"></i>
    </div>
    <h4 class="service-title">Dashboards & Reporting</h4>
    <p>Create interactive dashboards that track performance, monitor KPIs, and support decision-making.</p>
  </div>

</div>

---

## Featured Projects

Real-world projects designed to demonstrate data skills, business understanding, and technical execution.

<div class="entries-grid" style="display: grid; grid-template-columns: 1fr 1fr; gap: 1.5rem; margin-top: 1rem;">

  {% assign latest_projects = site.projects | sort: 'date' | reverse %}
  {% for project in latest_projects limit:2 %}
    <div class="card-hover">
      {% if project.image %}
        <img src="{{ project.image | relative_url }}" alt="{{ project.title }}" style="width: 100%; height: 180px; object-fit: cover; border-radius: 6px; margin-bottom: 0.5rem;" />
      {% endif %}
      <h3 style="margin-top: 0;">
        <a href="{{ project.link }}" target="_blank">{{ project.title }}</a>
      </h3>
      <p style="font-size: 0.85rem; color: #666;"><strong>{{ project.date | date: "%B %d, %Y" }}</strong></p>
      <p style="font-size: 0.9rem;">{{ project.description | truncatewords: 24 }}</p>
      <a href="{{ project.link }}" target="_blank" style="font-size: 0.85rem; color: #007ACC;">View project →</a>
    </div>
  {% endfor %}

</div>

<div style="margin-top: 1.5rem;">
  <a href="/projects" class="btn btn--primary">View All My Projects</a>
</div>

---

## Recent Blog Posts

Short reads on data, analytics, and cloud — written for clarity, insight, and real-world relevance.

<div class="entries-grid" style="display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 1.5rem; margin-top: 1.5rem;">

  {% for post in site.posts limit:3 %}
    <article class="card-hover">
      {% if post.header.image %}
        <img src="{{ post.header.image | relative_url }}" alt="{{ post.title }}" style="width: 100%; height: 180px; object-fit: cover; border-radius: 6px; margin-bottom: 0.75rem;" />
      {% else %}
        <img src="/assets/images/default-thumbnail.png" alt="Default" style="width: 100%; height: 180px; object-fit: cover; border-radius: 6px; margin-bottom: 0.75rem;" />
      {% endif %}

      <h4 style="margin-top: 0; font-size: 1.05rem;">
        <a href="{{ post.url | relative_url }}" style="color: #222; text-decoration: none;">{{ post.title }}</a>
      </h4>

      <p style="font-size: 0.85rem; color: #666;">{{ post.date | date: "%B %d, %Y" }}</p>

      {% if post.excerpt %}
        <p style="font-size: 0.9rem;">{{ post.excerpt | strip_html | truncatewords: 20 }}</p>
      {% endif %}

      <a href="{{ post.url | relative_url }}" style="font-size: 0.85rem; color: #007ACC;">Read more →</a>
    </article>
  {% endfor %}

</div>

<div style="margin-top: 1.5rem;">
  <a href="/notes" class="btn btn--primary">View All My Writings</a>
</div>

---

<style>
  .card-hover {
    border: 1px solid #ddd;
    border-radius: 8px;
    padding: 1rem;
    background-color: #fff;
    transition: all 0.3s ease;
  }

  .card-hover:hover {
    transform: translateY(-4px);
    box-shadow: 0 6px 16px rgba(0, 0, 0, 0.1);
  }

  .service-card {
    flex: 1 1 calc(48% - 1rem);
    min-width: 280px;
    border: 1px solid #ddd;
    padding: 1.25rem;
    border-radius: 8px;
    background-color: #f9f9f9;
    transition: all 0.3s ease;
  }

  .service-card:hover {
    background-color: #fff;
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.08);
    transform: translateY(-2px);
  }

  .service-title {
    font-size: 1.1rem;
    display: flex;
    align-items: center;
  }

  @media screen and (max-width: 768px) {
    .service-card {
      flex: 1 1 100%;
    }
  }
</style>
