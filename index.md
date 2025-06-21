---
layout: single
author_profile: true
---

👋 Hi! I’m Ocran, a data and analytics professional in training with a background in finance.

I use tools like Python, SQL, Excel, Power BI, and AWS to clean, explore, and visualize data in ways that solve real-world business problems.

Currently completing:
- DataCamp’s Data Science and Analytics tracks  
- Generation Ghana's Data Analyst Bootcamp  
- Hands-on cloud and analytics projects in finance and operations

📚 On this site, you’ll find:
- ✅ Data & cloud projects  
- ✍🏽 Insights from my learning journey (Data Notes)  
- 📜 Certifications and skills  
- 💡 Career growth stories

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
