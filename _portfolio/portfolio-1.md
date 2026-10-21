---
title: "Portfolio Robot Mobile"
excerpt: "BUT GEII 1re année, semestre 1 : mes traces pour les compétences Concevoir et Vérifier.<br/><img class='vignette' src='/mdb2/images/projets/robot-mobile/robot-mobile.jpg' alt='Le Robot Mobile'>"
collection: portfolio
---
{% include base_path %}

Ce portfolio rassemble mes traces de la SAÉ Robot Mobile, réalisée au premier semestre. Chaque trace est rattachée à un apprentissage critique (AC) du niveau 1 des compétences **Concevoir** et **Vérifier** du référentiel GEII.

<div class="fiche" markdown="1">
**Cadre** : BUT GEII 1re année, semestre 1, SAÉ 1.01 « Concevoir la partie GEII d'un système » et SAÉ 1.02 « Vérifier la partie GEII d'un système »<br>
**Équipe** : binôme avec [Martin Chevrollier](https://www.linkedin.com/in/martin-chevrollier/)<br>
**Le projet** : [Robot Mobile]({{ base_path }}/publications/2025-11-01-paper-title-number-1/)
</div>

## Concevoir la partie GEII d'un système

### AC11.01 · Produire une analyse fonctionnelle d'un système simple

<div class="activite-bloc">
<div class="activite-texte" markdown="1">
À partir du cahier des charges, nous avons rédigé le cahier d'exigences, puis découpé la carte en fonctions numérotées de FP1 à FP16.

Le schéma fonctionnel montre le chemin de chaque signal : capteur infrarouge, détection de seuil, abaisseur de tension vers la Raspberry Pi, puis commande des moteurs.
</div>
<figure class="activite-image">
  <a href="{{ base_path }}/images/portfolio/robot-mobile/schema-fonctionnel.png"><img src="{{ base_path }}/images/portfolio/robot-mobile/schema-fonctionnel.png" alt="Schéma fonctionnel du Robot Mobile, fonctions FP1 à FP16"></a>
  <figcaption>Trace : notre schéma fonctionnel</figcaption>
</figure>
</div>

### AC11.02 · Réaliser un prototype

Nous avons dessiné le schéma électrique sous KiCad, calculé les résistances du seuil de comparaison (2,6 V), puis routé et soudé la carte avant de la monter sur le robot.

<div class="activite-photos schemas trois">
  <figure>
    <a href="{{ base_path }}/images/projets/robot-mobile/schema-electrique.png"><img src="{{ base_path }}/images/projets/robot-mobile/schema-electrique.png" alt="Schéma électrique de la carte du Robot Mobile"></a>
    <figcaption>Schéma électrique sous KiCad</figcaption>
  </figure>
  <figure>
    <a href="{{ base_path }}/images/projets/robot-mobile/calcul-seuil.jpg"><img src="{{ base_path }}/images/projets/robot-mobile/calcul-seuil.jpg" alt="Calcul manuscrit des résistances du seuil"></a>
    <figcaption>Calcul des résistances du seuil</figcaption>
  </figure>
  <figure>
    <a href="{{ base_path }}/images/projets/robot-mobile/carte-montee.jpg"><img src="{{ base_path }}/images/projets/robot-mobile/carte-montee.jpg" alt="Notre carte montée sur le robot"></a>
    <figcaption>Le prototype monté sur le robot</figcaption>
  </figure>
</div>

### AC11.03 · Rédiger un dossier de fabrication

<div class="activite-bloc">
<div class="activite-texte" markdown="1">
Pour chaque fonction, nous avons listé les composants avec leur valeur, leur boîtier, les outils, la méthode de soudure et leur emplacement sur la carte.

Ce dossier nous a servi de guide pendant la soudure, fonction par fonction.
</div>
<figure class="activite-image">
  <a href="{{ base_path }}/images/portfolio/robot-mobile/fiche-fabrication.png"><img src="{{ base_path }}/images/portfolio/robot-mobile/fiche-fabrication.png" alt="Extrait du dossier de fabrication : liste des composants de la fonction FP7"></a>
  <figcaption>Trace : liste des composants de FP7</figcaption>
</figure>
</div>

## Vérifier la partie GEII d'un système

### AC12.01 · Appliquer une procédure d'essais

<div class="activite-bloc">
<div class="activite-texte" markdown="1">
Chaque fonction a été testée seule avec une fiche de test : rôle, points de mesure, appareils et résultats attendus.

Pour l'alimentation FA1, nous avons injecté 10 V au multimètre : la sortie donne bien 5 V. En polarité inversée, la sortie reste à 0 V et la carte est protégée.
</div>
<figure class="activite-image">
  <a href="{{ base_path }}/images/portfolio/robot-mobile/fiche-test-fa1.png"><img src="{{ base_path }}/images/portfolio/robot-mobile/fiche-test-fa1.png" alt="Fiche de test unitaire de la fonction FA1"></a>
  <figcaption>Trace : fiche de test de l'alimentation</figcaption>
</figure>
</div>

### AC12.02 et AC12.03 · Identifier et décrire un dysfonctionnement

<div class="activite-bloc">
<div class="activite-texte" markdown="1">
Lors des tests, les LED témoins des capteurs (FP2 et FP4) ne s'allumaient pas. Avec la fiche de dépannage, nous avons vérifié l'alimentation, puis le signal d'entrée et de sortie.

La cause était une mauvaise soudure. Nous avons remplacé les LED en respectant leur sens.
</div>
<figure class="activite-image">
  <a href="{{ base_path }}/images/portfolio/robot-mobile/fiche-depannage.png"><img src="{{ base_path }}/images/portfolio/robot-mobile/fiche-depannage.png" alt="Fiche de dépannage des fonctions FP2 et FP4"></a>
  <figcaption>Trace : fiche de dépannage FP2/FP4</figcaption>
</figure>
</div>

Bilan : je sais maintenant suivre le cycle en V de l'analyse jusqu'aux tests. Il me reste à mieux gérer le temps : toutes les soudures n'ont pas été finies, même si un moteur a tourné sur notre carte.
{: .notice}

<p><a class="btn btn--primary" href="{{ base_path }}/files/cahier-de-labo-robot-mobile.pdf">Lire le cahier de laboratoire (PDF)</a></p>

{% include style-blocs.html %}
