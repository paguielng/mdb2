---
permalink: /
title: "Accueil"
excerpt: "Étudiant en BUT GEII à Toulouse : électronique, informatique embarquée et automatisme."
author_profile: true
redirect_from:
  - /about/
  - /about.html
---
{% include base_path %}

<div class="hero">
  <p class="hero__title">Je conçois des systèmes électroniques qui fonctionnent pour de vrai.</p>
  <p class="hero__lead">Étudiant en <strong>BUT Génie Électrique et Informatique Industrielle (GEII)</strong> à Toulouse, je me spécialise dans l'électronique, l'informatique embarquée et l'automatisme industriel.</p>
  <p class="a-completer">Ce que tu recherches et à quelle date (ex. « Je recherche un stage de 10 semaines à partir d'avril 2027 » ou une alternance). C'est l'information que le recruteur doit voir en premier.</p>
  <a href="{{ base_path }}/projets/" class="btn btn--primary btn--large">Voir mes projets</a>
  <a href="{{ base_path }}/cv/" class="btn btn--outline btn--large">Mon CV</a>
  <a href="{{ base_path }}/contact/" class="btn btn--outline btn--large">Me contacter</a>
</div>

## Ce que je sais faire

<ul class="cards">
  <li class="card"><div class="card__body">
    <i class="fas fa-microchip card__icon" aria-hidden="true"></i>
    <h3 class="card__title">Électronique</h3>
    <p class="card__text">Schémas et cartes sous KiCad et Proteus, mesures à l'oscilloscope, Arduino et ESP32.</p>
  </div></li>
  <li class="card"><div class="card__body">
    <i class="fas fa-code card__icon" aria-hidden="true"></i>
    <h3 class="card__title">Informatique embarquée</h3>
    <p class="card__text">C/C++ sur microcontrôleur (STM32, Raspberry Pi), Python pour l'automatisation et l'analyse de données.</p>
  </div></li>
  <li class="card"><div class="card__body">
    <i class="fas fa-industry card__icon" aria-hidden="true"></i>
    <h3 class="card__title">Automatisme</h3>
    <p class="card__text">Programmation d'automates avec TIA Portal (Siemens) et Control Expert (Schneider Electric).</p>
  </div></li>
</ul>

## Projets à la une

{% include project-cards.html limit=3 %}

<p><a href="{{ base_path }}/projets/">Voir tous mes projets <i class="fas fa-arrow-right" aria-hidden="true"></i></a></p>

## En dehors des cours

Passionné d'aéronautique et d'espace depuis le collège (BIA, stage à l'ISAE-SUPAERO), j'ai conçu et lancé ma propre [micro-fusée]({{ base_path }}/projets/04-micro-fusee/) au Fablab de Planète Sciences. Je m'engage aussi comme bénévole auprès d'élèves de primaire avec l'AFEV, et j'ai été lauréat 2026 du prix **STEM for All** de Thales Solidarity. [Découvrir mes expériences]({{ base_path }}/experiences/).
