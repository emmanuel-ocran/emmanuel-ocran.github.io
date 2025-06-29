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
     class="btn btn--outline">Learn More About Me</a>
</div>

&nbsp;

## What I Do

<div class="service-grid">

  <div class="service-card" style="background-color: #E1F5FE;">
    <h4 class="service-title">Data Analysis & Visualization</h4>
    <p>Analyze, clean, and visualize data using Python, SQL, Excel, and Power BI to uncover business insights.</p>
  </div>

  <div class="service-card" style="background-color: #FCE4EC;">
    <h4 class="service-title">Cloud Data Workflows</h4>
    <p>Build automated pipelines with AWS (S3, Athena, Lambda) for scalable, cloud-native data reporting.</p>
  </div>

  <div class="service-card" style="background-color: #FFF9C4;">
    <h4 class="service-title">Business-Focused Analytics</h4>
    <p>Deliver end-to-end analytics solutions aligned with goals in finance, education, and development sectors.</p>
  </div>

  <div class="service-card" style="background-color: #E8F5E9;">
    <h4 class="service-title">Dashboards & Reporting</h4>
    <p>Create interactive dashboards that track performance, monitor KPIs, and support decision-making.</p>
  </div>

</div>

## Featured Projects

<div class="entries-grid">
  {% assign latest_projects = site.projects | sort: 'date' | reverse %}
  {% for project in latest_projects limit:2 %}
    <div class="card-hover">
      {% if project.image %}
        <img src="{{ project.image | relative_url }}" alt="{{ project.title }}" class="project-image" />
      {% endif %}
      <h3><a href="{{ project.link }}" target="_blank" class="link-blue">{{ project.title }}</a></h3>
      <p class="project-date">{{ project.date | date: "%B %d, %Y" }}</p>
      <p>{{ project.description | truncatewords: 24 }}</p>
      <a class="project-link" href="{{ project.link }}" target="_blank">View project →</a>
    </div>
  {% endfor %}
</div>

<div style="margin-top: 1.5rem;">
  <a href="/projects" class="btn btn--primary">View All My Projects</a>
</div>

## Recent Blog Posts

{% for post in site.posts %}
<div class="blog-post">
  {% if post.teaser %}
    <img src="{{ post.teaser  | relative_url }}" alt="{{ post.title }}" class="post-image" />
  {% else %}
    <img src="/assets/images/default-thumbnail.png" alt="Post image" class="post-image" />
  {% endif %}
  <div class="post-text">
    <h3><a href="{{ post.url | relative_url }}" class="link-blue">{{ post.title }}</a></h3>
    <p class="post-date">{{ post.date | date: "%B %d, %Y" }}</p>
    <p>{{ post.excerpt | strip_html | truncatewords: 25 }}</p>
  </div>
</div>
{% endfor %}

<div style="margin-top: 1.5rem;">
  <a href="/notes" class="btn btn--primary">View All My Writings</a>
</div>

<style>
  .entries-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 1.5rem;
    margin-top: 1rem;
  }

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

  .project-image, .post-image {
    width: 180px;
    height: 110px;
    object-fit: cover;
    border-radius: 6px;
  }

  .post-text {
    display: flex;
    flex-direction: column;
    justify-content: center;
  }

  .project-date, .post-date {
    font-size: 0.75rem;
    color: #666;
    margin-top: 0.25rem;
  }

  .project-link {
    font-size: 0.85rem;
    color: #007ACC;
    text-decoration: none;
    margin-top: 0.5rem;
    display: inline-block;
  }

  .blog-post {
    display: flex;
    flex-direction: row;
    gap: 1rem;
    margin-bottom: 2rem;
    border-bottom: 1px solid #ddd;
    padding-bottom: 1rem;
    align-items: center;
  }

  @media screen and (max-width: 768px) {
    .blog-post {
      flex-direction: column;
      align-items: flex-start;
    }
  }

  .service-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 1.5rem;
    margin-top: 1rem;
  }

  .service-card {
    border-radius: 10px;
    padding: 1.5rem;
    color: #333;
    transition: transform 0.3s ease;
  }

  .service-card:hover {
    transform: translateY(-3px);
    box-shadow: 0 4px 16px rgba(0,0,0,0.1);
  }

  .service-title {
    margin: 0;
    font-size: 1.1rem;
    font-weight: bold;
    margin-bottom: 0.5rem;
  }

  .btn--outline {
    border: 1px solid #007ACC;
    color: #007ACC;
    padding: 0.4rem 1rem;
    border-radius: 5px;
    text-decoration: none;
  }

  .btn--primary {
    background-color: #00BCD4;
    color: white;
    padding: 0.5rem 1.2rem;
    border: none;
    border-radius: 5px;
    text-decoration: none;
  }

  .link-blue {
    color: #007ACC;
    text-decoration: none;
  }
</style>
