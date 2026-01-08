---
layout: project
title: Vi-Notes
order: 8
summary: Authenticity verification platform that ensures genuine human writing through keyboard activity monitoring and statistical signature analysis
color: "FF6B6B"
repo: "vicharanashala/vi-notes"
features: []
---

## **Project Overview**

Vi-Notes verifies human-written content authenticity by monitoring writing in real-time. Users write freely while the platform captures keyboard activity patterns, typing rhythm, editing behaviors, and statistical signatures that distinguish genuine human composition from AI-generated or AI-assisted text.

## **Key Features**

The platform provides a distraction-free writing interface with silent background monitoring capturing typing speed, pause patterns, deletions, and composition rhythm. The keyboard monitoring tracks micro-patterns like hesitations before sentences, corrections during idea refinement, and variable typing speeds that reflect natural thinking processes.

Statistical analysis examines linguistic patterns, vocabulary diversity, sentence structure variations, and stylistic consistency. AI-generated text exhibits regularities like excessive consistency in sentence length or uniform vocabulary distribution that mismatch keyboard activity. After each session, Vi-Notes generates authenticity reports with confidence scores, suspicious patterns, and supporting evidence. Users share these reports to prove authorship in academic, professional, or publishing contexts. Real-time feedback flags unusual patterns like pasted text chunks or non-human typing behaviors.

## **Technologies Used**

Frontend: React, TypeScript, Electron for native desktop apps accessing keyboard events. Backend: Node.js, Express.js. OS-level APIs capture keystroke timing and patterns. ML models (TensorFlow, PyTorch) use supervised learning on human vs. AI text and unsupervised anomaly detection. NLP models analyze statistical signatures. MongoDB stores sessions, keystroke data, and reports with privacy-preserving encryption.

## **Detection Methods**

The system identifies behavioral patterns difficult for AI to replicate: natural sentence pauses, real-time corrections, variable typing speed based on cognitive load, and micro-pauses at punctuation. These signatures compare against known human patterns.

Text analysis reveals origin clues through variation in sentence length and structure, idiosyncratic vocabulary choices, and correlation between writing complexity and revision frequency. Human writers revise complex sections more than simple ones; AI-pasted text shows no such correlation.

Cross-referencing behavioral data with textual patterns provides the strongest verification. Paragraphs appearing without keystroke data, suspiciously constant typing speeds, or mismatched statistical signatures flag potential AI involvement.

## **Project Goals**

Vi-Notes restores trust in written content through reliable authorship verification, helping educators ensure academic integrity and enabling writers to prove authenticity. The platform develops accurate detection algorithms distinguishing human writing from various AI assistance levels while maintaining strict privacy protection. The system adapts continuously as AI writing tools evolve, staying ahead of new techniques attempting to mimic human writing patterns.

## **GitHub Repository**

[Vi-Notes](https://github.com/{{ page.repo }}){:target="_blank"}

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
