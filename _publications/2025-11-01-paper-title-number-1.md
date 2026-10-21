---
title: "Projet Robot Mobile 1"
collection: publications
category: manuscripts
permalink: /publication/2025-11-01-paper-title-number-1
excerpt: "Cette page présente la carte électronique d'un robot suiveur de ligne, conçue et testée selon le cycle en V."
date: 2025-11-01
membres: 'Paguiel Nganji, <a href="https://www.linkedin.com/in/martin-chevrollier/">Martin Chevrollier</a>'
paperurl: 'https://paguielng.github.io/mdb2/files/cahier-de-labo-robot-mobile.pdf'
citation: 'SAE Robot mobile, BUT GEII, 2025-2026, avec Martin Chevrollier.'
---

{% include base_path %}

<div class="fiche" markdown="1">
**Cadre** : SAE électronique du 1er semestre, BUT GEII, 2025-2026<br>
**Équipe** : binôme avec [Martin Chevrollier](https://www.linkedin.com/in/martin-chevrollier/)<br>
**Outils** : KiCad, simulation, alimentation de laboratoire, multimètre
</div>

## Le projet

Une usine veut un robot autonome pour acheminer ses pièces. Le robot suit une ligne noire et s'arrête sur une ligne transverse ; il doit tenir au moins 30 minutes sur sa batterie de 9,6 V. Notre mission : concevoir et tester la carte électronique de cette base roulante.


## Réalisation

### Conception de la carte

<div class="activite-bloc">
<div class="activite-texte" markdown="1">
Avec Martin Chevrollier, nous avons suivi le cycle en V : cahier d'exigences, analyse fonctionnelle, dimensionnement, mise en œuvre puis tests.

Notre carte, dessinée sous KiCad, alimente en 5 V les deux capteurs infrarouges, compare leur tension à un seuil réglable et commande les deux moteurs : l'un par un transistor bipolaire, l'autre par un MOSFET.
</div>
<figure class="activite-image">
  <img src="{{ base_path }}/images/projets/robot-mobile/robot-mobile.jpg" alt="Base roulante du Robot Mobile, deux roues motrices et une roue libre">
  <figcaption>La base roulante du Robot Mobile</figcaption>
</figure>
</div>

<div class="activite-photos schemas trois">
  <figure>
    <img src="{{ base_path }}/images/projets/robot-mobile/schema-electrique.png" alt="Schéma électrique de la détection de ligne et de la commande des moteurs">
    <figcaption>Schéma électrique sous KiCad</figcaption>
  </figure>
  <figure>
    <img src="{{ base_path }}/images/projets/robot-mobile/calcul-seuil.jpg" alt="Calcul manuscrit des résistances du seuil de comparaison">
    <figcaption>Calcul des résistances du seuil</figcaption>
  </figure>
  <figure>
    <img src="{{ base_path }}/images/projets/robot-mobile/carte-3d.png" alt="Vue 3D de la carte du Robot Mobile">
    <figcaption>Vue 3D de notre carte</figcaption>
  </figure>
</div>

Dimensionnement : le seuil de comparaison est réglé à 2,6 V, environ au milieu du potentiomètre, ce que la simulation a confirmé avant la soudure.
{: .notice}

### Fabrication et tests

<div class="activite-bloc">
<div class="activite-texte" markdown="1">
Chaque fonction a été soudée puis testée seule, avec une fiche de test. L'alimentation donne bien 5 V, et en cas d'inversion de polarité la carte reste protégée. Les capteurs donnent environ 4,9 V sur fond clair et 0 V sur fond foncé, comme prévu.

Nous n'avons pas eu le temps de finir toutes les soudures, mais un moteur a tourné sur notre carte.
</div>
<figure class="activite-image">
  <img src="{{ base_path }}/images/projets/robot-mobile/carte-montee.jpg" alt="Notre carte montée sur le robot, à côté de la Raspberry Pi et de sa carte Sense HAT">
  <figcaption>Notre carte montée sur le robot</figcaption>
</figure>
</div>

Dépannage : les LED des capteurs ne s'allumaient pas. La cause était une mauvaise soudure ; nous les avons remplacées en respectant leur sens.
{: .notice}

Bilan : coût estimé à 452,83 € pour 100 cartes (composants et circuit imprimé). Sans les moteurs, la carte consomme 40,4 mA.
{: .notice}

<p><a class="btn btn--primary" href="{{ base_path }}/files/cahier-de-labo-robot-mobile.pdf">Lire le cahier de laboratoire (PDF)</a></p>

{% include style-blocs.html %}
