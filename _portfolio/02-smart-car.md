---
title: "Smart Car pilotée par smartphone"
excerpt: "SAÉ S2 : transformer une voiture radiocommandée en voiture connectée en Bluetooth, avec anticollision et alertes sonores."
categorie: "SAÉ"
order: 2
header:
  teaser: projets/smart-car.jpg
redirect_from:
  - /portfolio/portfolio-2/
  - /publication/2026-01-01-paper-title-number-3
---
{% include base_path %}


<div class="fiche">
  <div><strong>Contexte</strong>SAÉ, BUT GEII semestre 2</div>
  <div><strong>Équipe</strong><span class="a-completer">seul, binôme ?</span></div>
  <div><strong>Mon rôle</strong><span class="a-completer">ce que tu as pris en charge</span></div>
  <div><strong>Outils</strong>Proteus, pont en H L298, capteurs IR Sharp, Bluetooth</div>
</div>

## L'objectif

Un fabricant de jouets veut moderniser une de ses voitures radiocommandées : on retire toute l'électronique d'origine pour en faire une voiture **pilotée depuis un smartphone** grâce à un joystick virtuel en Bluetooth. La voiture doit aussi **prendre seule certaines décisions** : ralentir puis freiner à l'approche d'un obstacle, prévenir le pilote par des bips, allumer ses phares quand il fait sombre.

<figure class="illustration">
  <img src="{{ base_path }}/images/1781005864267.jpg" alt="Schéma fonctionnel de la Smart Car : capteurs, moteurs, phares et liaison smartphone">
  <figcaption>Architecture fonctionnelle de la voiture : capteurs avant/arrière, moteurs de propulsion et de direction, phares et liaison avec le smartphone.</figcaption>
</figure>

## Ce que j'ai fait

<p class="a-completer">Explique ta contribution directe avec « je » : quelle partie tu as conçue (carte électronique, programme, appli smartphone…), un moment difficile et la solution trouvée. Ajoute une photo de TA voiture ou de ta carte, avec une légende.</p>

## Le résultat

<p class="a-completer">La démonstration a-t-elle fonctionné ? Quelles fonctions marchaient (anticollision, klaxon, phares auto, bargraphe, température) ? Autonomie mesurée ?</p>

## Ce que j'ai appris

**Compétences techniques** : <span class="a-completer">ex. commande de moteurs avec un pont en H, mesure de distance, communication Bluetooth, conception de carte sous Proteus</span>

**Compétences transversales** : <span class="a-completer">ex. organisation, gestion des priorités, documentation technique</span>

<details class="cahier-des-charges">
<summary>Voir le cahier des charges du projet</summary>

<p><strong>Matériel ajouté</strong> : module pont en H L298 (moteurs de direction et de propulsion), buzzer passif, deux capteurs infrarouges Sharp, batterie de 6 accumulateurs NiMH 1,2 V 2300 mAh ou pack 2 × 18650 Li-ion.</p>

<p><strong>Fonctions attendues</strong> :</p>
<ul>
  <li>pilotage par joystick virtuel sur smartphone via Bluetooth ;</li>
  <li>détection d'obstacle avant et arrière en trois zones (près &lt; 40 cm, moyen 40 à 60 cm, loin) ;</li>
  <li>bips de plus en plus rapides à l'approche d'un obstacle, klaxon prioritaire ;</li>
  <li>vitesse réduite de 50 % en zone moyenne, freinage maximal en zone proche ;</li>
  <li>phares avant et arrière en mode ON ou AUTO (capteur de luminosité), feux arrière renforcés au freinage ;</li>
  <li>bargraphe virtuel (obstacle ou niveau de batterie) et température extérieure affichés sur le téléphone.</li>
</ul>

<p><strong>Livrables</strong> : dossier de fabrication (cahier, GERBER, fichier Proteus), dossier technique, prototype opérationnel, coût unitaire pour 100 exemplaires, étude d'autonomie (au moins 30 minutes).</p>

<p><strong>Volume horaire</strong> : 2 h de cours, 28 h de TD, 27 h de TP, 25 h en autonomie.</p>
</details>
