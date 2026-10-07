---
title: "Robot mobile suiveur de ligne"
excerpt: "SAÉ S1 en binôme : concevoir l'électronique et programmer une base roulante autonome sur Raspberry Pi."
categorie: "SAÉ"
order: 1
header:
  teaser: projets/robot-mobile.jpg
redirect_from:
  - /portfolio/portfolio-1/
  - /publication/2025-11-01-paper-title-number-1
  - /publication/2025-12-01-paper-title-number-2
---
{% include base_path %}


<div class="fiche">
  <div><strong>Contexte</strong>SAÉ, BUT GEII semestre 1</div>
  <div><strong>Équipe</strong>Binôme</div>
  <div><strong>Mon rôle</strong><span class="a-completer">ce que tu as pris en charge</span></div>
  <div><strong>Outils</strong>Raspberry Pi, Sense HAT, capteurs IR, KiCad / Proteus</div>
</div>

## L'objectif

Une usine veut un petit robot capable d'acheminer des pièces d'assemblage **en toute autonomie**. Notre mission : concevoir, vérifier et valider l'électronique puis la programmation d'une base roulante qui suit une ligne au sol, avec au moins **30 minutes d'autonomie** sur une batterie 9,6 V / 2300 mAh.

<figure class="illustration">
  <img src="{{ base_path }}/images/ROMO-LineTracker.png" alt="Robot mobile équipé d'une Raspberry Pi posé sur une piste à ligne noire">
  <figcaption>Le robot sur la piste : Raspberry Pi, carte Sense HAT (compas) et deux capteurs infrarouges de suivi de ligne.</figcaption>
</figure>

## Ce que j'ai fait

<p class="a-completer">Raconte les étapes en disant « je » : ce que tu as conçu ou programmé toi-même (schéma, carte, code de suivi de ligne, tests…), un problème rencontré et comment tu l'as résolu.</p>

1. **Partie électronique** : <span class="a-completer">ex. schéma, choix des composants, routage, calcul du coût pour 100 cartes</span>
2. **Partie informatique** : <span class="a-completer">ex. lecture des capteurs, algorithme de suivi, utilisation du compas</span>
3. **Tests et démonstration** : <span class="a-completer">ex. réglages sur la piste, résultat de la démo finale</span>

## Ce que j'ai appris

**Compétences techniques** : <span class="a-completer">2 ou 3 compétences que tu sais maintenant refaire seul</span>

**Compétences transversales** : travail en binôme, partage du robot entre équipes (organisation du temps), tenue d'un cahier de laboratoire à chaque séance. <span class="a-completer">confirme ou ajuste, et ajoute ce que tu en retiens personnellement</span>

<details class="cahier-des-charges">
<summary>Voir le cahier des charges du projet</summary>

<p><strong>Livrables attendus</strong> : un prototype opérationnel, un dossier de fabrication (cahier de fabrication et fichiers GERBER), un dossier technique (cahier de laboratoire et documentation) et une démonstration.</p>

<p><strong>Existant</strong> : plateforme à deux roues motorisées et une roue libre, deux capteurs de suivi de ligne infrarouge, Raspberry Pi et carte Sense HAT avec fonction compas.</p>

<p><strong>Contraintes</strong> : autonomie d'au moins 30 minutes (batterie 9,6 V, 2300 mAh) ; calcul du coût unitaire de l'électronique pour 100 cartes ; travail en binôme avec robot partagé ; cahier de laboratoire mis à jour sur Teams à chaque séance.</p>

<p><strong>Volume horaire</strong> : 1 h de cours, 22 h de TD, 26 h de TP, 12 h en autonomie.</p>
</details>
