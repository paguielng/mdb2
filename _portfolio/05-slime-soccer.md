---
title: "Slime Soccer, jeu de football 2D"
excerpt: "Projet personnel : un jeu d'arcade jouable dans le navigateur, avec un moteur physique fait maison (React et Canvas)."
categorie: "Projet personnel"
order: 5
header:
  teaser: https://github.com/paguielng/rxeus/blob/main/assets/pitch.png?raw=true
redirect_from:
  - /talks/2014-02-01-talk-2
  - /posts/2012/08/blog-post-4/
---

<div class="fiche">
  <div><strong>Type</strong>Jeu web</div>
  <div><strong>Technologies</strong>React, Canvas 2D</div>
  <div><strong>Jouer</strong><a href="https://rxeus.netlify.app/">rxeus.netlify.app</a></div>
  <div><strong>Code</strong><a href="https://github.com/paguielng/rxeus/">github.com/paguielng/rxeus</a></div>
</div>

## L'objectif

Recréer le classique jeu de navigateur *Slime Soccer* (Quin Pendragon) : deux « slimes » s'affrontent pour envoyer la balle dans le but adverse. Le défi était surtout de programmer une **physique crédible** : gravité, rebonds, collisions et transfert de vitesse entre le slime et la balle.

<figure class="illustration">
  <img src="https://github.com/paguielng/rxeus/blob/main/assets/pitch.png?raw=true" alt="Terrain de Slime Soccer avec les deux slimes et la balle">
  <figcaption>Le terrain : slime cyan à gauche, slime rouge à droite, buts avec filets de chaque côté.</figcaption>
</figure>

## Comment ça marche

- Une **boucle de jeu** à 60 images par seconde (`requestAnimationFrame`) : mise à jour de la physique, puis dessin sur le canvas.
- Des **constantes physiques** réglées à la main : gravité, puissance du saut, amortissement de l'air et perte d'énergie à chaque rebond.
- Une **détection de collision** basée sur la distance entre les centres de la balle et du slime.
- Des matchs chronométrés de 1 à 8 minutes, un mode 2 joueurs sur le même clavier et un mode contre l'ordinateur.

## Ce que j'ai appris

<p class="a-completer">Ce que ce projet t'a apporté (ex. traduire des lois physiques en code, déboguer une animation, publier un site en ligne). Précise aussi comment tu l'as réalisé (seul, avec un tutoriel, avec l'aide d'une IA ?) pour rester transparent.</p>
