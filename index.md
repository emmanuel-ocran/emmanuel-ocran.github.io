---
layout: single
title: "Home"
author_profile: true
---

&nbsp;  
&nbsp;


I'm a data analyst with a background in finance, specializing in data visualization, cloud analytics, and insight generation.  
I turn raw business data into clear, actionable insights using tools like Python, SQL, Power BI, and Excel.  
With growing cloud expertise in AWS, I'm building scalable, insight-driven solutions that bridge data and business needs.  
Currently focused on real-world projects and sharing practical lessons through my portfolio and Data Notes.


&nbsp;  
&nbsp;


---

### ⚒️ Tech Stack:
**Languages:** Python, SQL  
**Tools:** Excel, Power BI, Jupyter Notebook  
**Cloud:** AWS (S3, Lambda), GitHub  
**Skills:** Data Cleaning, Storytelling, Dashboards

📫 [Contact me](mailto:mrocran1@gmail.com) or connect via [LinkedIn](https://linkedin.com/in/emmanuel-ocran)

---

## 🔥 Recent Posts

{% for post in site.posts limit:3 %}
### [{{ post.title }}]({{ post.url | relative_url }})
<small><strong>{{ post.date | date: "%B %d, %Y" }}</strong> — {{ post.reading_time }} read</small>

{{ post.excerpt }}

[Read more]({{ post.url | relative_url }})  
---
{% endfor %}
