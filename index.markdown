---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---
# Welcome to NPTEL Winter Internship 2025

**Organized by NPTEL** — Master full-stack development with the MERN stack under the guidance of **Prof. Sudarshan Iyengar** at IIT Ropar's Vicharanashala Lab. This intensive program covers TypeScript, React, Express.js, and MongoDB through hands-on case studies and real-world projects, bringing together 400+ learners from across India.


**Quick Guide:** To get a complete overview of the program structure and learning journey, start with the [Introduction](./intro/). Review the [FAQ](./faq/) to understand detailed policies and answers to common questions. For the latest updates, deadlines, important messages, and upcoming activities, regularly check the [Announcements](./announcements/). Track your learning progress, submission status, and performance metrics in real time using the [Live Dashboards](./Dashboard.html). Visit the [Case Studies](./case-studies/) section for hands-on MERN practice problems, and explore the [Projects](./projects/) section to discover and track the larger internship projects you may choose to work on. For additional references, guides, and helpful materials, explore [Genie](./genie/) from the navigation menu.


## 📊 Live Dashboard

➡️ [Open Live Dashboard](./Dashboard.html)

## 📢 Announcements

{% assign announcements_page = site.pages | where: "permalink", "/announcements/" | first %}
{% for announcement in announcements_page.announcements limit:2 %}
{{ forloop.index }}. **[{{ announcement.title }}](./announcements/)** ({{ announcement.date }})  
   {{ announcement.description | truncatewords: 20 }}
{% endfor %}

➡️ [View All Announcements](./announcements/)

<!-- ---
[Important Links](./important_links/) -->