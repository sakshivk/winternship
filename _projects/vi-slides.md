---
layout: project
title: Vi-SlideS
order: 7
summary: AI-powered adaptive classroom platform that tailors teaching based on student questions and cognitive analysis
color: "FFFF00"
repo: "vicharanashala/vi-slides"
features: []
---

## **Project Overview**

Vi-SlideS revolutionizes teaching by making it question-driven and adaptive. After a brief 5-10 minute topic introduction, students submit questions that shape class direction. AI analyzes collective questions, providing teachers with real-time insights into class mood, motivation, and conceptual understanding. AI automatically addresses straightforward questions, allowing teachers to focus on complex queries requiring deeper explanation and personalized attention.

## **Key Features**

Students submit questions after the topic introduction through a real-time interface. They can choose anonymous or identified submissions and track question status to see which AI answered versus teacher-addressed. AI detects overall class mood by examining sentiment and tone, assesses motivation levels, classifies questions by cognitive level, extracts main themes and concerns, and identifies learning gaps.

The system performs smart triage to determine auto-answerable questions versus those needing teacher attention. Straightforward questions get instant AI responses with relevant sources. Complex questions route to the teacher's prioritized dashboard. Teachers see real-time question overviews, class insights (mood, motivation, knowledge gaps), AI-prioritized questions, and suggested teaching direction. They can review and override AI answers as needed.

## **Technologies Used**

### Current Testing Phase
Google Forms for question collection, Google Sheets for data aggregation and analysis, Google Slides for presentation and visualization.

### Planned Stack
Frontend: React, TypeScript. Backend: Express.js, Node.js. Database: MongoDB. AI/NLP: LLMs for question analysis and response generation. Sentiment analysis: NLP models for mood and motivation detection. Classification models for cognitive complexity assessment. Real-time communication: WebSockets.

## **System Workflow**

Pre-class: Teacher presents 5-10 minute overview; students submit questions. AI Analysis: System collects questions, classifies by complexity, analyzes sentiment for mood/motivation, creates gist of understanding and concerns. Response: Straightforward questions get instant AI responses; complex questions route to prioritized teacher dashboard; teacher uses insights to guide discussion dynamically. Post-class: System generates comprehensive analytics report; questions/answers archived for future reference.

## **Question Classification**

AI auto-answers factual or definition-based queries, previously answered similar questions, and low cognitive complexity clarifications. Teachers address questions with high conceptual depth, novel perspectives, complex problem-solving scenarios, personalized explanation needs, and critical thinking queries.

## **Project Goals**

Vi-SlideS transforms traditional lectures into question-driven, adaptive learning experiences where student curiosity shapes class direction. The platform provides real-time insights into understanding and engagement, reducing teacher burden through automated responses and enabling focus on complex discussions. The responsive teaching approach improves engagement as students see their questions influencing class content. Identifying learning gaps early helps address problems before they become ingrained. The platform creates data-driven teaching strategies based on question analysis, fostering more interactive and student-centered classrooms.

## **GitHub Repository**

[Vi-SlideS](https://github.com/{{ page.repo }}){:target="_blank"}

{% if page.features.size > 0 %}
## **Upcoming Features**

{% for feature in page.features %}
<details style="margin-bottom: 1.5rem; border-radius: 12px; overflow: hidden; box-shadow: 0 4px 12px rgba(0,0,0,0.1);">
<summary style="cursor: pointer; padding: 1rem 1.5rem; background: linear-gradient(135deg, #{{ page.color }}20 0%, #{{ page.color }}40 100%); border-left: 6px solid #{{ page.color }}; font-weight: 600; list-style: none;">&nbsp;{{ feature.title }}</summary>
<div style="padding: 1.5rem; background-color: white;">
{{ feature.description }}
<br><br>
<a href="https://github.com/{{ page.repo }}/issues/{{ feature.issue }}" target="_blank" style="color: #{{ page.color }}; font-weight: 600; text-decoration: none;">View Feature Request #{{ feature.issue }} →</a>
</div>
</details>
{% endfor %}
{% endif %}
