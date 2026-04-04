---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% include base_path %}

{% for paper in site.data.publications %}
<div class="publication-entry">
  <h3 class="publication-title">{{ paper.title }}</h3>
  <p class="publication-meta">{{ paper.venue }} • {{ paper.year }}</p>
  <div class="publication-figure">
    <img src="/{{ paper.figure }}" alt="{{ paper.title }}">
  </div>
  <p class="publication-summary">{{ paper.summary }}</p>
  {% if paper.url %}
  <p class="publication-links">
    <a href="{{ paper.url }}" target="_blank">Paper</a>
  </p>
  {% endif %}
</div>
{% endfor %}
