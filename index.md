---
layout: single
title: ""
author_profile: true
classes: wide
---

<!-- Hero Section -->
&nbsp;

Hi! I'm **Emmanuel Ocran** — associate data scientist and analyst.

I help businesses and nonprofits make smarter decisions by transforming complex data into clear, actionable insights.

With a background in finance and growing expertise in cloud analytics, I design scalable solutions that simplify reporting, uncover trends, and drive measurable impact.

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
    <h4 class="service-title"><i class="fas fa-chart-line service-icon"></i> Data Analysis & Visualization</h4>
    <p>Using Python, SQL, Excel, and Power BI to explore, clean, and visualize data to uncover insights.</p>
  </div>

  <div class="service-card">
    <h4 class="service-title"><i class="fas fa-cloud service-icon"></i> Cloud-Based Workflows</h4>
    <p>Building scalable data pipelines with AWS tools like S3, Athena, and Lambda for efficient reporting.</p>
  </div>

  <div class="service-card">
    <h4 class="service-title"><i class="fas fa-briefcase service-icon"></i> Business-Focused Analytics</h4>
    <p>Delivering data solutions in finance, education, and development sectors that drive business outcomes.</p>
  </div>

  <div class="service-card">
    <h4 class="service-title"><i class="fas fa-tachometer-alt service-icon"></i> Insightful Dashboards</h4>
    <p>Designing performance dashboards that help teams track KPIs, identify patterns, and make better decisions.</p>
  </div>

</div>

## Latest Projects

A snapshot of the projects I've been working on

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
      {% if project.skills %}
        <div class="tag-list">
          {% for skill in project.skills %}
            <span class="tag">{{ skill }}</span>
          {% endfor %}
        </div>
      {% endif %}
      <a href="{{ project.link }}" target="_blank" style="font-size: 0.85rem; color: #007ACC;">View project →</a>
    </div>
  {% endfor %}

</div>

<div style="margin-top: 1.5rem;">
  <a href="/projects" class="btn btn--primary">View All My Projects</a>
</div>

## Recent Posts

My latest thoughts and insights

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

      {% if post.tags %}
        <div class="tag-list">
          {% for tag in post.tags %}
            <span class="tag">{{ tag }}</span>
          {% endfor %}
        </div>
      {% endif %}

      <a href="{{ post.url | relative_url }}" style="font-size: 0.85rem; color: #007ACC;">Read more →</a>
    </article>
  {% endfor %}

</div>

<div style="margin-top: 1.5rem;">
  <a href="/notes" class="btn btn--primary">View All My Writings</a>
</div>

<!-- Styles -->
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

  .tag-list {
    margin: 0.5rem 0;
  }

  .tag {
    display: inline-block;
    background-color: #f1f1f1;
    border-radius: 4px;
    font-size: 0.75rem;
    padding: 0.25rem 0.5rem;
    margin: 0.15rem;
    color: #333;
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
