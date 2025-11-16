---
layout: single
title: "Academic Career"
permalink: /academic/
author_profile: true
---

{% assign cv = site.data.cv %}

<p>This page summarizes my academic career, including degrees and thesis topic. Entries are synced from <a href="{{ site.baseurl }}/cv-json/">the JSON CV</a>.</p>

{% if cv.education and cv.education.size > 0 %}
<ul class="cv-list">
  {% for edu in cv.education %}
  <li class="cv-item">
    <div class="cv-item-header">
      <div class="cv-item-title">{{ edu.area }}</div>
      <div class="cv-item-date">{{ edu.startDate }}{% if edu.endDate %} – {{ edu.endDate }}{% else %} – Present{% endif %}</div>
    </div>
    <div class="cv-item-content">
      <div class="cv-item-subtitle">{{ edu.institution }}</div>
      {% if edu.subject %}
      <div class="cv-item-detail"><strong>Subject:</strong> {{ edu.subject }}</div>
      {% endif %}
      {% if edu.supervisors and edu.supervisors.size > 0 %}
      <div class="cv-item-detail"><strong>Supervisors:</strong> {{ edu.supervisors | join: ", " }}</div>
      {% endif %}
    </div>
  </li>
  {% endfor %}
</ul>
{% else %}
<p>No academic entries found.</p>
{% endif %}
