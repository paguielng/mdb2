---
title: "Projet Line Tracker 2"
collection: publications
category: manuscripts
permalink: /publication/2025-12-01-paper-title-number-2
excerpt: "Cette page présente la partie numérique du robot suiveur de ligne, pilotée par une Raspberry Pi."
date: 2025-12-01
membres: 'Paguiel Nganji, <a href="https://www.linkedin.com/in/martin-chevrollier/">Martin Chevrollier</a>'
citation: 'SAE Line Tracker, BUT GEII, 2025-2026, avec Martin Chevrollier.'
---

{% include base_path %}

<div class="fiche" markdown="1">
**Cadre** : SAE informatique du 1er semestre, BUT GEII, 2025-2026<br>
**Équipe** : binôme avec [Martin Chevrollier](https://www.linkedin.com/in/martin-chevrollier/)<br>
**Matériel** : Raspberry Pi, carte Sense HAT (compas), capteurs infrarouges de ligne
</div>

## Le projet

<div class="activite-bloc">
<div class="activite-texte" markdown="1">
C'est la suite du [Robot Mobile]({{ base_path }}/publication/2025-11-01-paper-title-number-1) : la même base roulante, mais cette fois pilotée par une **Raspberry Pi**. La carte Sense HAT ajoute un compas qui donne le cap suivi par le robot.

Le robot doit suivre une ligne noire sur fond clair de façon plus fine qu'en mode purement analogique.
</div>
<figure class="activite-image">
  <img src="{{ base_path }}/images/projets/line-tracker/robot.jpg" alt="Le robot suiveur de ligne avec sa Raspberry Pi, sa carte Sense HAT et sa nappe de liaison">
  <figcaption>Le robot et sa Raspberry Pi</figcaption>
</figure>
</div>

## Ce que nous avons fait

Avec Martin, nous avons travaillé sur les capteurs optiques, l'asservissement du robot et l'optimisation du suivi de trajectoire, puis nous avons validé le comportement par des tests sur la piste.

{% include style-blocs.html %}
