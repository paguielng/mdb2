---
title: "Portfolio SMART CAR"
excerpt: "BUT GEII 1re année, semestre 2 : mes traces pour les compétences Concevoir et Vérifier.<br/><img class='vignette' src='/mdb2/images/projets/smartcar/smartcar.jpg' alt='La SmartCar'>"
collection: portfolio
---
{% include base_path %}

Ce portfolio rassemble mes traces de la SAÉ SmartCar, réalisée au second semestre. La SAÉ 2.01 mobilise les six apprentissages critiques (AC) du niveau 1 des compétences **Concevoir** et **Vérifier** du référentiel GEII.

<div class="fiche" markdown="1">
**Cadre** : BUT GEII 1re année, semestre 2, SAÉ 2.01 « Conception et vérification d'un prototype à partir d'un cahier des charges complet »<br>
**Équipe** : binôme avec [Pierre Gazeau](https://www.linkedin.com/in/pierre-gazeau-5631b0361/)<br>
**Le projet** : [SmartCar]({{ base_path }}/publications/2026-01-01-paper-title-number-3/)
</div>

## Concevoir la partie GEII d'un système

### AC11.01 · Produire une analyse fonctionnelle d'un système simple

<div class="activite-bloc">
<div class="activite-texte" markdown="1">
Le cahier des charges est plus complet qu'au premier semestre : détection d'obstacles, sons, phares, température et niveau de batterie.

Nous l'avons traduit en exigences, puis en fonctions FP1 à FP11 reliées à la carte microcontrôleur. Côté programme, chaque fonction a sa vue externe : entrées, sorties et rôle.
</div>
<figure class="activite-image">
  <a href="{{ base_path }}/images/portfolio/smartcar/schema-fonctionnel.png"><img src="{{ base_path }}/images/portfolio/smartcar/schema-fonctionnel.png" alt="Schéma fonctionnel de la carte électronique de la SmartCar"></a>
  <figcaption>Trace : notre schéma fonctionnel</figcaption>
</figure>
</div>

### AC11.02 · Réaliser un prototype matériel et logiciel

Le prototype est à la fois une carte et un programme : une carte shield pour la Nucleo STM32, simulée sous Proteus, et un code C++ écrit sous PlatformIO à partir de nos algorithmes.

<div class="activite-photos schemas trois">
  <figure>
    <a href="{{ base_path }}/images/projets/smartcar/carte-shield-3d.jpg"><img src="{{ base_path }}/images/projets/smartcar/carte-shield-3d.jpg" alt="Vue 3D de la carte shield de la SmartCar"></a>
    <figcaption>Vue 3D de la carte shield</figcaption>
  </figure>
  <figure>
    <a href="{{ base_path }}/images/portfolio/smartcar/algorithme-propulsion.png"><img src="{{ base_path }}/images/portfolio/smartcar/algorithme-propulsion.png" alt="Algorithme de la fonction pwm_propulsion"></a>
    <figcaption>Algorithme de la propulsion</figcaption>
  </figure>
  <figure>
    <a href="{{ base_path }}/images/projets/smartcar/smartcar.jpg"><img src="{{ base_path }}/images/projets/smartcar/smartcar.jpg" alt="La SmartCar avec sa carte montée sur le toit"></a>
    <figcaption>Le prototype final</figcaption>
  </figure>
</div>

L'algorithme de propulsion décide seul de freiner : si un obstacle approche par l'arrière, la voiture freine, même si le joystick demande de reculer.
{: .notice}

### AC11.03 · Rédiger un dossier de fabrication

<div class="activite-bloc">
<div class="activite-texte" markdown="1">
Pour chaque fonction, le dossier donne la référence, la valeur, la technologie (traversante ou CMS), le boîtier, les outils et la méthode de soudure.

Chaque composant est repéré en couleur sur le schéma d'implantation, ce qui a évité les erreurs de placement.
</div>
<figure class="activite-image">
  <a href="{{ base_path }}/images/portfolio/smartcar/fiche-fabrication.png"><img src="{{ base_path }}/images/portfolio/smartcar/fiche-fabrication.png" alt="Extrait du dossier de fabrication : composants de la fonction FP7"></a>
  <figcaption>Trace : composants de la fonction FP7</figcaption>
</figure>
</div>

## Vérifier la partie GEII d'un système

### AC12.01 · Appliquer une procédure d'essais

<div class="activite-bloc">
<div class="activite-texte" markdown="1">
Chaque fonction a sa fiche de test. Pour l'alimentation FA1, nous attendions 5 V et une référence de 2,5 V : nous avons mesuré 5,1 V et 2,493 V, avec la LED allumée.

Les signaux PWM de propulsion ont été relevés à l'oscilloscope pour vérifier leur fréquence et leur rapport cyclique.
</div>
<figure class="activite-image">
  <a href="{{ base_path }}/images/portfolio/smartcar/fiche-test-fa1.png"><img src="{{ base_path }}/images/portfolio/smartcar/fiche-test-fa1.png" alt="Fiche de test unitaire de la fonction FA1 de la SmartCar"></a>
  <figcaption>Trace : fiche de test de l'alimentation</figcaption>
</figure>
</div>

### AC12.02 et AC12.03 · Identifier et décrire un dysfonctionnement

<div class="activite-bloc">
<div class="activite-texte" markdown="1">
La fonction FP11 (niveau de batterie) donnait 3,4 V au lieu des 3,3 V attendus. L'alimentation, les entrées et les soudures étaient correctes.

Nous avons trouvé deux causes : un arrondi dans le calcul du pont diviseur, et des noms de résistances différents entre KiCad et la carte. Après recalcul, nous avons soudé R4 = 18 kΩ et R40 = 3,3 kΩ.
</div>
<figure class="activite-image">
  <a href="{{ base_path }}/images/portfolio/smartcar/fiche-depannage.png"><img src="{{ base_path }}/images/portfolio/smartcar/fiche-depannage.png" alt="Fiche de dépannage de la fonction FP11"></a>
  <figcaption>Trace : fiche de dépannage FP11</figcaption>
</figure>
</div>

Bilan : par rapport au Robot Mobile, j'ai ajouté la partie logicielle et mené un vrai dépannage jusqu'à la cause. J'ai aussi appris à garder les mêmes noms de composants du schéma jusqu'à la carte.
{: .notice}

<p class="bc-docs">
  <a class="btn btn--primary" href="{{ base_path }}/files/cahier-de-labo-smartcar-electronique.pdf">Cahier de labo : électronique (PDF)</a>
  <a class="btn btn--primary" href="{{ base_path }}/files/cahier-de-labo-smartcar-info-embarquee.pdf">Cahier de labo : informatique embarquée (PDF)</a>
</p>

{% include style-blocs.html %}
