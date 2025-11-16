---
permalink: /
title: "Abderrahim Akhrouf — PhD in Fluid Mechanics"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
feature_row:
  - title: "Thesis: ML + EIT"
    excerpt: "Optimizing electric pump energy consumption with EIT and machine learning."
    url: "/thesis/"
    btn_label: "Explore Thesis"
    btn_class: "btn--primary"
  - title: "Professional Experience"
    excerpt: "PhD research and prior AI/control internships."
    url: "/experience/"
    btn_label: "View Experience"
  - title: "Academic Career"
    excerpt: "PhD and earlier studies — supervisors and subject."
    url: "/academic/"
    btn_label: "View Academic Path"
---


Welcome — I'm Abderrahim Akhrouf, a PhD candidate in Fluid Mechanics. I build machine learning models and apply electrical impedance tomography to improve pump energy efficiency and real-time monitoring. This site highlights my thesis, publications, and experience.

<div class="hero">
  <div class="container">
    <h1 class="hero__title">Optimizing energy consumption in electric pumps</h1>
    <p class="hero__subtitle">Combining electrical impedance tomography with machine learning to monitor and optimize pump performance. Explore the thesis summary and code below.</p>
    <a class="btn btn--primary" href="{{ site.baseurl }}/thesis/" aria-label="Read thesis">Read Thesis</a>
    <a class="btn btn--inverse" href="{{ site.baseurl }}/publications/" aria-label="Open publications">Publications</a>
    <a class="btn" href="mailto:abderrahim.akhrouf@etu.univ-amu.fr" aria-label="Contact by email">Contact</a>
  </div>
</div>

<div class="affiliations" aria-label="Affiliations">
  <a class="badge badge--logo" href="https://www.univ-amu.fr/en" target="_blank" rel="noopener" aria-label="Aix-Marseille University">
    <img src="{{ '/images/affiliations/amu.svg' | relative_url }}" alt="Aix-Marseille University logo" />
    <span>Aix-Marseille University</span>
  </a>
  <a class="badge badge--logo" href="https://www.lma.cnrs-mrs.fr/" target="_blank" rel="noopener" aria-label="Laboratory of Mechanics and Acoustics, CNRS">
    <img src="{{ '/images/affiliations/lma.svg' | relative_url }}" alt="LMA (CNRS) logo" />
    <span>LMA (CNRS)</span>
  </a>
  <a class="badge badge--logo" href="https://www.fluiidd.fr/" target="_blank" rel="noopener" aria-label="FLUIIDD">
    <img src="{{ '/images/affiliations/fluiidd.svg' | relative_url }}" alt="FLUIIDD logo" />
    <span>FLUIIDD</span>
  </a>
</div>

{% include feature_row %}

### Latest Publication
{% assign latest_pub = site.publications | sort: 'date' | last %}
{% if latest_pub %}
<div class="archive__item" style="margin-top: 0.5rem;">
  <div class="archive__item-body">
    <h2 class="archive__item-title" style="margin-bottom: .25rem;">
      <a href="{{ latest_pub.url | relative_url }}">{{ latest_pub.title }}</a>
    </h2>
    {% if latest_pub.venue %}<p style="margin: 0 0 .25rem 0;">{{ latest_pub.venue }}</p>{% endif %}
    {% if latest_pub.excerpt %}<p style="margin: 0 0 .5rem 0;">{{ latest_pub.excerpt }}</p>{% endif %}
    {% if latest_pub.paperurl %}<a class="btn btn--primary" href="{{ latest_pub.paperurl }}" target="_blank" rel="noopener">Read Paper</a>{% endif %}
  </div>
  </div>
{% endif %}

### Core Skills
<p>
  <span class="btn">Machine Learning</span>
  <span class="btn">Deep Learning</span>
  <span class="btn">Reinforcement Learning</span>
  <span class="btn">Time-series</span>
  <span class="btn">EIT</span>
  <span class="btn">Python</span>
  <span class="btn">MATLAB</span>
</p>
