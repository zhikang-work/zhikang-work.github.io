---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: true
---

{% include base_path %}

{% for project in site.data.projects %}
<div class="project-entry">
  <h3 class="project-title">{{ project.title }}</h3>
  <p class="project-meta">{{ project.meta }}</p>
  {% if project.image %}
  <div class="project-figure">
    <img src="/{{ project.image }}" alt="{{ project.title }}">
  </div>
  {% endif %}
  <p class="project-summary">{{ project.summary }}</p>
  {% if project.url %}
  <p class="project-links">
    <a href="{{ project.url }}" target="_blank">Project Details</a>
  </p>
  {% endif %}
</div>
{% endfor %}

## Academic Service

Peer reviewer for major conferences including CVPR, ICCV, ECCV, NeurIPS, AAAI, WACV, and ACL. Recognized as an **Outstanding Reviewer** (top 5%) at **CVPR 2025**.
