---
permalink: /
title: "Bienvenue dans mon garage"
layout: splash
author_profile: false
redirect_from: 
  - /about/
  - /about.html
feature_row:
  - image_path: accueil/chaine-de-production.jpg
    alt: "Chaîne de production automatisée en salle de TP"
    title: "Chaîne de production"
    excerpt: "SAE automatisme et informatique industrielle, avec mon cahier de laboratoire."
    url: "/publication/2026-06-01-paper-title-number-4"
    btn_label: "Voir le projet"
    btn_class: "btn--primary"
  - image_path: accueil/line-tracker.jpg
    alt: "Robot suiveur de ligne avec sa carte Raspberry Pi"
    title: "Line Tracker"
    excerpt: "SAE informatique : un robot qui suit une ligne au sol."
    url: "/publication/2025-12-01-paper-title-number-2"
    btn_label: "Voir le projet"
    btn_class: "btn--primary"
  - image_path: accueil/micro-fusee.jpg
    alt: "Micro-fusée tenue en main avant le lancement"
    title: "Micro-fusée"
    excerpt: "Projet personnel : conception, simulation et premier vol."
    url: "/talks/2012-03-01-talk-1"
    btn_label: "Voir le projet"
    btn_class: "btn--primary"
---

{% include base_path %}

<section class="bc-hero">
  <img class="bc-hero__photo" src="{{ base_path }}/images/{{ site.author.avatar }}" alt="Photo de {{ site.author.name }}">
  <h1 class="bc-hero__title">Bienvenue dans mon garage</h1>
<div class="bc-hero__text" markdown="1">
Je suis [Paguiel Nganji](https://www.linkedin.com/in/paguiel-nganji/), étudiant en **Génie électrique et informatique industrielle**, et je suis passionné par le fonctionnement des systèmes. Je me spécialise dans l'électronique, l'informatique embarquée et l'automatisme industriel.

Ce site présente mes travaux universitaires et mes projets personnels. Vous trouverez d'autres exemples de mon travail sur mon [profil GitHub](https://github.com/paguielng), comme des projets expérimentaux et de petits gadgets électroniques. Chaque projet est l'occasion d'apprendre une nouvelle façon de réfléchir et de faire les choses.
</div>
  <p class="bc-hero__actions">
    <a class="btn btn--primary" href="{{ base_path }}/publications/">Voir mes projets</a>
    <a class="bc-link" href="{{ base_path }}/cv/">Lire mon CV</a>
  </p>
</section>

<section class="bc-section">
  <h2 class="bc-section__title">Mes projets phares</h2>
  {% include feature_row %}
</section>

<section class="bc-band">
<div class="bc-band__inner" markdown="1">
## Mes outils

Dans mon travail, j'ai l'habitude d'utiliser certains outils :
{: .bc-band__lead}

- [C/C++](https://isocpp.org/) pour les applications embarquées où les performances sont cruciales
- [KiCad](https://www.kicad.org/) pour schématiser les circuits électroniques
- [Proteus](https://www.labcenter.com/) pour la conception et simulation de circuits imprimés simplifiées
- [Git/GitHub](https://github.com/paguielng/) pour gérer mes projets
- [Wokwi](https://wokwi.com/) pour simuler des circuits électroniques et de microcontrôleurs des ESP32
- [MATLAB](https://www.mathworks.com/products/matlab.html) pour résoudre des nombres complexes et des calculs matriciels
- [Fusion 360](https://www.autodesk.com/fr/products/fusion-360/overview/) pour la modélisation CAO
{: .bc-checks}
</div>
</section>
