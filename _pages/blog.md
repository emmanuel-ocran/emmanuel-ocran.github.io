---
layout: single
title: ""
permalink: /blog/
entries_layout: list
author_profile: true
description: "Personal blog by Emmanuel Ocran — sharing practical insights on data, cloud, and analytics."
---

<img src="/assets/images/banners/dn-banner.jpg" 
     alt="Data Notes Cover"
     style="width: 100%; height: 250px; object-fit: cover; border-radius: 8px; margin-bottom: 1rem;" />


**Welcome to my blog**

A space where I share practical notes, and reflections from working in data, cloud, and analytics. From quick ideas to deeper insights, this blog captures my learning journey, tools explored, and practical takeaways.

Looking for weekly curated insights instead?  
👉 [Subscribe to the Data Notes Newsletter](https://www.linkedin.com/newsletters/data-notes-1234567890)


---

{% for post in site.posts %}
<div style="display: flex; gap: 1rem; margin-bottom: 2rem; border-bottom: 1px solid #ddd; padding-bottom: 1rem;">
  {% if post.teaser %}
    <img src="{{ post.teaser  | relative_url }}" alt="{{ post.title }}" style="width: 180px; height: 110px; object-fit: cover; border-radius: 6px;" />
  {% else %}
    <img src="/assets/images/default-thumbnail.png" alt="Post image" style="width: 180px; height: 110px; object-fit: cover; border-radius: 6px;" />
  {% endif %}

  <div>
    <h3 style="margin-top: 0;"><a href="{{ post.url | relative_url }}" style="color: #007ACC;">{{ post.title }}</a></h3>
    <p style="margin: 0.2rem 0; color: #666; font-size: 0.9rem;">{{ post.date | date: "%B %d, %Y" }}</p>
    <p style="margin: 0; font-size: 0.95rem;">{{ post.excerpt | strip_html | truncatewords: 25 }}</p>
    <a href="{{ post.url | relative_url }}" style="font-size: 0.85rem;">Read more →</a>
  </div>
</div>
{% endfor %}