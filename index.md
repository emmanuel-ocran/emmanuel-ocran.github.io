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

<div class="service-grid">

  <div class="service-card" style="background-color: #FFF6DD;">
    <div class="service-icon">📈</div>
    <h4 class="service-title">Strategy & Planning</h4>
    <ul>
      <li>Time for lead research, work</li>
      <li>Traders & Stocks</li>
      <li>Business Opportunities</li>
    </ul>
    <a class="service-button" href="#">Get Details →</a>
  </div>

  <div class="service-card" style="background-color: #D9F5EC;">
    <div class="service-icon">💼</div>
    <h4 class="service-title">Investment Policy</h4>
    <ul>
      <li>Time for lead research, work</li>
      <li>Traders & Stocks</li>
      <li>Business Opportunities</li>
    </ul>
    <a class="service-button" href="#">Get Details →</a>
  </div>

  <div class="service-card" style="background-color: #FFE5EB;">
    <div class="service-icon">🧾</div>
    <h4 class="service-title">Tax Management</h4>
    <ul>
      <li>Time for lead research, work</li>
      <li>Traders & Stocks</li>
      <li>Business Opportunities</li>
    </ul>
    <a class="service-button" href="#">Get Details →</a>
  </div>

  <div class="service-card" style="background-color: #FFF3DE;">
    <div class="service-icon">💰</div>
    <h4 class="service-title">Financial Advice</h4>
    <ul>
      <li>Time for lead research, work</li>
      <li>Traders & Stocks</li>
      <li>Business Opportunities</li>
    </ul>
    <a class="service-button" href="#">Get Details →</a>
  </div>

</div>

---

## Featured Projects

<div class="entries-grid">
  {% assign latest_projects = site.projects | sort: 'date' | reverse %}
  {% for project in latest_projects limit:2 %}
    <div class="card-hover">
      {% if project.image %}
        <img src="{{ project.image | relative_url }}" alt="{{ project.title }}" class="project-image" />
      {% endif %}
      <h3><a href="{{ project.link }}" target="_blank">{{ project.title }}</a></h3>
      <p class="project-date"><strong>{{ project.date | date: "%B %d, %Y" }}</strong></p>
      <p>{{ project.description | truncatewords: 24 }}</p>
      <a class="project-link" href="{{ project.link }}" target="_blank">View project →</a>
    </div>
  {% endfor %}
</div>

<div style="margin-top: 1.5rem;">
  <a href="/projects" class="btn btn--primary">View All My Projects</a>
</div>

---

## Recent Blog Posts

{% for post in site.posts %}
<div class="blog-post">
  {% if post.teaser %}
    <img src="{{ post.teaser  | relative_url }}" alt="{{ post.title }}" class="post-image" />
  {% else %}
    <img src="/assets/images/default-thumbnail.png" alt="Post image" class="post-image" />
  {% endif %}
  <div>
    <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
    <p class="post-date">{{ post.date | date: "%B %d, %Y" }}</p>
    <p>{{ post.excerpt | strip_html | truncatewords: 25 }}</p>
  </div>
</div>
{% endfor %}

<div style="margin-top: 1.5rem;">
  <a href="/notes" class="btn btn--primary">View All My Writings</a>
</div>

---

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
    width: 100%;
    height: 180px;
    object-fit: cover;
    border-radius: 6px;
    margin-bottom: 0.5rem;
  }

  .project-date, .post-date {
    font-size: 0.85rem;
    color: #666;
  }

  .project-link, .service-button {
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
  }

  @media screen and (max-width: 768px) {
    .blog-post {
      flex-direction: column;
    }
  }

  .service-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
    gap: 1.5rem;
    margin-top: 1rem;
  }

  .service-card {
    border-radius: 10px;
    padding: 1rem;
    color: #333;
    transition: transform 0.3s ease;
  }

  .service-card:hover {
    transform: translateY(-3px);
    box-shadow: 0 4px 16px rgba(0,0,0,0.1);
  }

  .service-icon {
    font-size: 1.5rem;
    margin-bottom: 0.5rem;
  }

  .service-title {
    margin: 0;
    font-size: 1.1rem;
    font-weight: bold;
  }

  .service-card ul {
    padding-left: 1.2rem;
    margin-top: 0.5rem;
    margin-bottom: 0.5rem;
  }
</style>
