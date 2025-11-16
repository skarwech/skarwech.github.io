---
permalink: /fr/
title: "Abderrahim Akhrouf — Doctorant en Mécanique des Fluides"
lang: fr
ref: home
author_profile: true
feature_row:
  - title: "Thèse : IA + TIE"
    excerpt: "Optimisation énergétique des pompes électriques par tomographie d'impédance et apprentissage automatique."
    url: "/thesis/" # (Pourrait pointer vers une version FR ultérieure)
    btn_label: "Explorer la thèse"
    btn_class: "btn--primary"
  - title: "Expérience Professionnelle"
    excerpt: "Recherche doctorale et stages en IA / contrôle."
    url: "/experience/"
    btn_label: "Voir l'expérience"
  - title: "Parcours Académique"
    excerpt: "Doctorat et études antérieures — sujets et encadrants."
    url: "/academic/"
    btn_label: "Voir le parcours"
---

{% include lang-switch.html %}

Bienvenue — Je suis Abderrahim Akhrouf, doctorant en mécanique des fluides. J'utilise l'apprentissage automatique et la tomographie d'impédance électrique pour améliorer l'efficacité énergétique et le suivi en temps réel des pompes électriques. Ce site présente ma thèse, mes publications et mon parcours.

<div class="hero">
  <div class="container">
    <h1 class="hero__title">Optimisation énergétique des pompes électriques</h1>
    <p class="hero__subtitle">Combiner la tomographie d'impédance électrique et l'apprentissage automatique pour surveiller et optimiser la performance des pompes.</p>
    <a class="btn btn--primary" href="{{ site.baseurl }}/thesis/" aria-label="Lire la thèse">Lire la thèse</a>
    <a class="btn btn--inverse" href="{{ site.baseurl }}/publications/" aria-label="Ouvrir publications">Publications</a>
    <a class="btn" href="mailto:abderrahim.akhrouf@etu.univ-amu.fr" aria-label="Contact par email">Contact</a>
  </div>
</div>

<div class="affiliations" aria-label="Affiliations">
  <a class="badge badge--logo" href="https://www.univ-amu.fr/" target="_blank" rel="noopener" aria-label="Aix-Marseille Université">
    <img src="{{ '/images/affiliations/amu.svg' | relative_url }}" alt="Logo AMU" />
    <span>Aix-Marseille Université</span>
  </a>
  <a class="badge badge--logo" href="https://www.lma.cnrs-mrs.fr/" target="_blank" rel="noopener" aria-label="Laboratoire de Mécanique et d'Acoustique, CNRS">
    <img src="{{ '/images/affiliations/lma.svg' | relative_url }}" alt="Logo LMA CNRS" />
    <span>LMA (CNRS)</span>
  </a>
  <a class="badge badge--logo" href="https://www.fluiidd.fr/" target="_blank" rel="noopener" aria-label="FLUIIDD">
    <img src="{{ '/images/affiliations/fluiidd.svg' | relative_url }}" alt="Logo FLUIIDD" />
    <span>FLUIIDD</span>
  </a>
</div>

{% include feature_row %}

### Dernière Publication
{% assign latest_pub = site.publications | sort: 'date' | last %}
{% if latest_pub %}
<div class="archive__item" style="margin-top: 0.5rem;">
  <div class="archive__item-body">
    <h2 class="archive__item-title" style="margin-bottom: .25rem;">
      <a href="{{ latest_pub.url | relative_url }}">{{ latest_pub.title }}</a>
    </h2>
    {% if latest_pub.venue %}<p style="margin: 0 0 .25rem 0;">{{ latest_pub.venue }}</p>{% endif %}
    {% if latest_pub.excerpt %}<p style="margin: 0 0 .5rem 0;">{{ latest_pub.excerpt }}</p>{% endif %}
    {% if latest_pub.paperurl %}<a class="btn btn--primary" href="{{ latest_pub.paperurl }}" target="_blank" rel="noopener">Lire l'article</a>{% endif %}
  </div>
  </div>
{% endif %}

### Compétences Clés
<p>
  <span class="btn">Apprentissage automatique</span>
  <span class="btn">Deep Learning</span>
  <span class="btn">Apprentissage par renforcement</span>
  <span class="btn">Séries temporelles</span>
  <span class="btn">Tomographie d'impédance</span>
  <span class="btn">Python</span>
  <span class="btn">MATLAB</span>
</p>
