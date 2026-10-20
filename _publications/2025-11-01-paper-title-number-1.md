---
title: "Projet Robot Mobile 1"
collection: publications
category: manuscripts
permalink: /publication/2025-11-01-paper-title-number-1
excerpt: 'Cette page traite le Cahier des charges : Robot Mobile (Électronique).'
date: 2025-11-01
venue: 'Journal 1'
membres: 'Paguiel Nganji, Martin Chevrollier'
slidesurl: 'https://paguielng.github.io/mdb2/files/slides1.pdf'
paperurl: 'https://paguielng.github.io/mdb2/files/paper1.pdf'
bibtexurl: 'https://paguielng.github.io/mdb2/files/bibtex1.bib'
citation: 'Paguiel, Martin. (2025). &quot;Projet Robot Mobile 1.&quot; <i>Journal 1</i>. 1(1).'
---

1. Présentation du projet
   ---
1.1 Contexte
   ---
Une entreprise souhaite développer un nouveau produit à destination de son usine de production pour acheminer
des pièces d'assemblage, en toute autonomie. Il est demandé de développer ce produit et de fournir :
- Un prototype
- Un dossier de fabrication (Cahier de fabrication + fichiers GERBER)
- Un dossier technique (cahier de laboratoire + documentation technique + )
- Une démonstration du système opérationnel
  
1.2 Objectifs
---

Concevoir, vérifier et valider l'électronique et la programmation d'une base roulante intelligente.

1.3 Description de l’existant
---
Le Robot est une plateforme dotée de 2 roues motorisées, d'une roue libre (bille) et de deux capteurs de suivi de
ligne infrarouge.
Vous avez à votre disposition un système Raspberry pi et une carte Sense HAT avec une fonction de compas qui
donne le cap suivi par le robot.

1.4 Critères d’acceptabilité du projet
---
- Dossier de fabrication complet
- Cahier de laboratoire complet et soigné
- Le robot est opérationnel
- Les consignes ont été respectées

2 Expression des besoins
   ---
2.1 Besoins fonctionnel
   ---
- Un prototype
- Un dossier technique (cahier de laboratoire)
- Une démonstration du système opérationnel

3 Contraintes
---
3.1 Coûts
   ---
Aucune contrainte de coût n’est imposée. En revanche un calcul de coût unitaire de l'électronique pour une
production de 100 cartes est attendu (Composants électroniques + circuit imprimé).

3.2 Autonomie de fonctionnement
---
La Base Roulante (robot) doit avoir une autonomie d'au moins 30 minutes avec une batterie de
2300mAh de 9,6V.

3.3 Délais de réalisation
---
1h C / 22h TD / 26h TP / 12h autonomie

3.4 Autres contraintes
---
- travail en binôme
- time sharing (robot partagé)
- cahier de laboratoire / de suivi à mettre à jour en fin de CHAQUE séance sur TEAMS

4 Déroulement du projet
---
4.1 Séquencement
   ---
- Partie électronique du projet
- Partie Numérique du projet

{% include base_path %}

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

<div class="activite-photos schemas">
  <figure>
    <img src="{{ base_path }}/images/projets/robot-mobile/schema-electrique.png" alt="Schéma électrique de la détection de ligne et de la commande des moteurs">
    <figcaption>Schéma électrique sous KiCad</figcaption>
  </figure>
  <figure>
    <img src="{{ base_path }}/images/projets/robot-mobile/calcul-seuil.jpg" alt="Calcul manuscrit des résistances du seuil de comparaison">
    <figcaption>Calcul des résistances du seuil</figcaption>
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
  <img class="activite-image" src="{{ base_path }}/images/projets/robot-mobile/carte-3d.png" alt="Vue 3D de la carte du Robot Mobile">
  <figcaption>Vue 3D de notre carte</figcaption>
</figure>
</div>

Dépannage : les LED des capteurs ne s'allumaient pas. La cause était une mauvaise soudure ; nous les avons remplacées en respectant leur sens.
{: .notice}

Bilan : coût estimé à 452,83 € pour 100 cartes (composants et circuit imprimé). Sans les moteurs, la carte consomme 40,4 mA.
{: .notice}

{% include style-blocs.html %}
