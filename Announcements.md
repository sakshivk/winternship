---
layout: page
title: Announcements
permalink: /announcements/
order: 1
announcements:
  - title: "The Self-Healing Endorsement Network"
    date: "January 9, 2026"
    description: "Understanding the endorsement network system, audit process, incentives, and dashboard challenge for visualizing endorsement chains and network health."
    content: |
      **Step 1: Understand the network**
      
      The Endorsement Network functions on a simple rule: students can endorse each other. Crucially, every line of endorsements must ultimately link back to a Jedi holder, who possesses the Gold, Silver, and Bronze tiers. The more students connected to a Jedi holder, the higher their reputation. Any groups that fail to connect to a Jedi holder form "floating islands" and are deemed inactive within the system.
      
      **Step 2: Follow endorsement rules**
      
      Students are restricted to receiving only one endorsement, yet they have the freedom to provide multiple endorsements to others. Crucially, any endorsement can only be made after the associated task or case study has been successfully finished.
      
      **Step 3: Know how audits work**
      
      Bhavna conducts audits to detect defaulters. If a defaulter is found, the entire endorsement path connected to that person is checked. A 50% penalty is applied to everyone in that connected group. The defaulter and anyone who fails the audit are removed from the network. Anyone Bhavna certifies as "good" can be recruited by anyone. Gold ticket holders can assist Bhavna during audits.
      
      **Step 4: Understand incentives**
      
      Whenever a new person joins a connected group, everyone in that group receives a 5% health point increase. This increase is calculated as 5% of their current health points plus 5% of the new member's health points.
      
      **Step 5: Work with the data**
      
      Students will be given a simple three-column dataset: Member 1, Member 2, and Action.
      
      The action can be added (Member 1 endorsed Member 2), deleted (Member 1 de-endorsed Member 2), or default (Member 1 is a defaulter and Member 2 is the parent).
      
      **Step 6: Your challenge**
      
      Using this data, students must create a dashboard that visualizes endorsement chains, penalties, incentives, and overall network health. The design and style are completely open-ended.

      ***Form for Endorsement's* [Endorse here](https://forms.gle/BfSfhWbxaMnqbWBa6){:target="_blank"}**
---

[← Back]({{ site.baseurl }}/)

## 📢 Latest Announcements

{% if page.announcements.size > 0 %}
{% for announcement in page.announcements %}

---

### {{ announcement.title }}

**📅 {{ announcement.date }}**

{% if announcement.content %}
{{ announcement.content }}
{% else %}
{{ announcement.description }}
{% endif %}

{% endfor %}
{% else %}
<div style="text-align: center; padding: 40px; color: #666;">
  <p style="font-size: 1.2em;">📭 No announcements at the moment</p>
  <p>Check back later for updates!</p>
</div>
{% endif %}

---

[← Back]({{ site.baseurl }}/)
