---
layout: single
title: "Professional Experience"
permalink: /experience/
author_profile: true
---

{% assign cv = site.data.cv %}

<p>Below is a curated view of my professional experience pulled from my CV data. It stays in sync with <a href="{{ site.baseurl }}/cv-json/">the JSON CV</a>.</p>

{% if cv.work and cv.work.size > 0 %}
<ul class="cv-list">
  {% for item in cv.work %}
  <li class="cv-item">
    <div class="cv-item-header">
      <div class="cv-item-title">{{ item.position }}</div>
      <div class="cv-item-date">{{ item.startDate }}{% if item.endDate %} – {{ item.endDate }}{% else %} – Present{% endif %}</div>
    </div>
    <div class="cv-item-content">
      <div class="cv-item-subtitle">{{ item.institution }}{% if item.location %} — {{ item.location }}{% endif %}</div>
      {% if item.summary %}
      <div class="cv-item-detail">{{ item.summary }}</div>
      {% endif %}
      {% if item.supervisors and item.supervisors.size > 0 %}
      <div class="cv-item-detail"><strong>Supervisors:</strong> {{ item.supervisors | join: ", " }}</div>
      {% endif %}
    </div>
  </li>
  {% endfor %}
</ul>
{% else %}
<p>No experience entries found.</p>
{% endif %}
