---
title: "Micro-fusée amateur"
excerpt: "Projet personnel au Fablab Planète Sciences : concevoir, simuler, fabriquer et lancer une micro-fusée de 60 cm (apogée 200 m)."
categorie: "Projet personnel"
order: 4
header:
  teaser: projets/micro-fusee.jpg
redirect_from:
  - /talks/2012-03-01-talk-1
---
{% include base_path %}

<div class="fiche">
  <div><strong>Cadre</strong>Le Fabriquet, Planète Sciences Occitanie</div>
  <div><strong>Période</strong>Fin 2022, lancement le 4 février 2023</div>
  <div><strong>Résultat</strong>Vol stable, apogée 200 m, parachute déployé</div>
  <div><strong>Outils</strong>Fusion 360, OpenRocket, StabTraj, impression 3D</div>
</div>

## L'objectif

Concevoir puis lancer **ma propre micro-fusée** d'environ 60 cm <span class="a-completer">ta capture OpenRocket indique 90 cm et une apogée simulée de 259 m : vérifie les chiffres</span>, en respectant le cahier des charges des campagnes de lancement de Planète Sciences : stabilité, résistance de la structure, système de récupération et sécurité.

<figure class="illustration">
  <img src="{{ base_path }}/images/projets/micro-fusee.jpg" alt="Micro-fusée rouge et blanche tenue juste avant le lancement">
  <figcaption>La micro-fusée terminée, juste avant le lancement à Bourg-Saint-Bernard.</figcaption>
</figure>

## Les étapes

### 1. Concevoir et simuler

J'ai modélisé la coiffe en 3D sous **Fusion 360**, puis simulé le vol complet dans **OpenRocket** : trajectoire, apogée, vitesse et position du centre de gravité (CG) par rapport au centre de poussée (CP). J'ai ensuite vérifié la conformité au cahier des charges avec **StabTraj**, le tableur de Planète Sciences qui calcule la finesse, la portance et la marge statique.

<figure class="illustration">
  <img src="{{ base_path }}/images/projets/micro-fusee-simulation.png" alt="Capture d'écran d'OpenRocket et du tableur StabTraj pour la fusée PAGrocket">
  <figcaption>À gauche, ma fusée dans OpenRocket avec les positions du CG et du CP ; à droite, la vérification dans le tableur Planète Sciences (marge statique, finesse, portance) qui conclut « STABLE ».</figcaption>
</figure>

### 2. Fabriquer

- **Coiffe** imprimée en 3D en PLA : léger, rigide et facile à imprimer.
- **Corps** en tube de carton renforcé, léger et économique.
- **Quatre ailerons** en bois fin, dimensionnés grâce aux simulations pour garder une marge statique positive.
- **Parachute** d'environ 15 cm, calculé pour une descente lente sans trop dériver avec le vent.

### 3. Lancer

Le 4 février 2023, sur l'aérodrome de Bourg-Saint-Bernard, la fusée a décollé de façon stable, atteint une **apogée de 200 mètres** et le parachute s'est ouvert comme prévu. Le vol a confirmé les choix faits pendant les simulations.

<figure class="illustration">
  <img src="{{ base_path }}/images/projets/micro-fusee-lancement.jpg" alt="Préparation de la rampe de lancement sur le terrain avec un encadrant">
  <figcaption>Préparation de la rampe de lancement avec un encadrant de Planète Sciences.</figcaption>
</figure>

## Ce que j'ai appris

**Compétences techniques** : modélisation CAO, simulation de vol, lecture d'un cahier des charges, impression 3D.

**Compétences transversales** : <span class="a-completer">ex. persévérance, respect des règles de sécurité, écoute des conseils des encadrants. Qu'est-ce qui t'a le plus marqué dans ce projet ?</span>

## Fichiers du projet

- [Ma simulation OpenRocket (.ork)]({{ base_path }}/files/micro-fusee/PAGrocket.ork)
- [Mon fichier StabTraj (.xls)]({{ base_path }}/files/micro-fusee/Logiciel_stabtraj_PAGrocket_modifie.xls)

<details class="cahier-des-charges">
<summary>Sources consultées</summary>
<ul>
  <li><a href="https://www.planete-sciences.org/espace/spock/">Planète Sciences, StabTraj (SPOCK)</a></li>
  <li><a href="https://www.planete-sciences.org/espace/IMG/pdf/cdc_minif.pdf">Planète Sciences, cahier des charges des minifusées</a></li>
  <li><a href="https://www.planete-sciences.org/espace/Microfusee/Presentation">Planète Sciences, présentation des microfusées</a></li>
  <li><a href="https://openrocket.info/">OpenRocket</a> et sa <a href="https://openrocket.readthedocs.io/en/latest/">documentation</a></li>
  <li><a href="https://www.youtube.com/watch?v=1XS6q_AbjtI">Stabilité des micro-fusées (vidéo)</a></li>
  <li><a href="https://berryrocket.com/micro_mystic.html">Berry Rocket, Micro Mystic</a></li>
</ul>
</details>
