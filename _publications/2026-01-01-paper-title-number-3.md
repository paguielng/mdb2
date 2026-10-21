---
title: "Projet SAE SMARTCAR 3"
collection: publications
category: manuscripts
permalink: /publication/2026-01-01-paper-title-number-3
excerpt: "Cette page présente une voiture pilotée par smartphone, avec anticollision, phares automatiques et avertisseur sonore."
date: 2026-01-01
membres: 'Paguiel Nganji, <a href="https://www.linkedin.com/in/pierre-gazeau-5631b0361/">Pierre Gazeau</a>'
paperurl: 'https://paguielng.github.io/mdb2/files/cahier-de-labo-smartcar-electronique.pdf'
citation: 'SAE SmartCar, BUT GEII, 2025-2026, avec Pierre Gazeau.'
---

{% include base_path %}

<div class="fiche" markdown="1">
**Cadre** : SAE du 2e semestre, BUT GEII, 2025-2026, menée selon le cycle en V<br>
**Équipe** : binôme avec [Pierre Gazeau](https://www.linkedin.com/in/pierre-gazeau-5631b0361/)<br>
**Outils** : Proteus, KiCad, carte Nucleo STM32, C++ sous PlatformIO, RemoteXY, oscilloscope
</div>

## Le projet

Un fabricant de jouets veut transformer une voiture radiocommandée en voiture pilotée par smartphone, en Bluetooth. Elle doit détecter les obstacles à l'avant et à l'arrière, ralentir puis freiner seule, biper de plus en plus vite et allumer ses phares quand il fait sombre.

## Réalisation

### Partie électronique

<div class="activite-bloc">
<div class="activite-texte" markdown="1">
Avec Pierre Gazeau, nous avons conçu une carte shield qui se branche sur une carte Nucleo STM32 et se loge sur le toit de la voiture.

Nous avons dimensionné, simulé sous Proteus puis testé chaque fonction : alimentation, détection de distance avant et arrière, capteurs de luminosité et de température, générateur audio à NE555 et mesure du niveau de batterie.
</div>
<figure class="activite-image">
  <img src="{{ base_path }}/images/projets/smartcar/smartcar.jpg" alt="La voiture SMARTCAR avec sa carte électronique montée sur le toit">
  <figcaption>Notre SMARTCAR avec sa carte shield</figcaption>
</figure>
</div>

Dépannage : le niveau de batterie mesuré valait 3,4 V au lieu de 3,3 V. Un arrondi dans nos calculs avait faussé les résistances ; après recalcul, nous avons soudé R4 = 18 kΩ et R40 = 3,3 kΩ.
{: .notice}

### Partie informatique embarquée

<div class="activite-bloc">
<div class="activite-texte" markdown="1">
J'ai programmé la carte en C++ sous PlatformIO. Le joystick de l'application RemoteXY pilote la direction et la vitesse par des signaux PWM, avec une zone morte de 10&nbsp;% au centre.

Le programme gère aussi le bargraphe de batterie, les bips du buzzer selon la distance de l'obstacle, les phares automatiques, le freinage anticollision et l'affichage de la température.
</div>
<figure class="activite-image">
  <img src="{{ base_path }}/images/projets/smartcar/application-remotexy.png" alt="Interface RemoteXY sur smartphone avec joystick et bargraphe de batterie">
  <figcaption>L'application de pilotage sur smartphone</figcaption>
</figure>
</div>

<div class="activite-photos schemas">
  <figure>
    <img src="{{ base_path }}/images/projets/smartcar/carte-shield-3d.jpg" alt="Vue 3D de la carte shield de la SMARTCAR">
    <figcaption>Vue 3D de la carte shield</figcaption>
  </figure>
  <figure>
    <img src="{{ base_path }}/images/projets/smartcar/pwm-oscilloscope.png" alt="Signaux PWM de propulsion relevés à l'oscilloscope">
    <figcaption>Signaux PWM de propulsion à l'oscilloscope</figcaption>
  </figure>
</div>

Bilan : coût estimé à 1 287,41 € pour 100 cartes. La carte consomme 86,65 mA, soit environ 30 h d'autonomie voiture à l'arrêt avec une batterie de 2600 mAh.
{: .notice}

<p class="bc-docs">
  <a class="btn btn--primary" href="{{ base_path }}/files/cahier-de-labo-smartcar-electronique.pdf">Cahier de labo : électronique (PDF)</a>
  <a class="btn btn--primary" href="{{ base_path }}/files/cahier-de-labo-smartcar-info-embarquee.pdf">Cahier de labo : informatique embarquée (PDF)</a>
</p>

{% include style-blocs.html %}
