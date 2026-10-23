---
layout: archive
title: "CV"
permalink: /cv/
redirect_from:
  - /resume
---

{% include base_path %}

Profil
======
Étudiant en 2e année de BUT GEII, parcours Électronique et Systèmes Embarqués. Je mesure, je teste et je valide : oscilloscope, multimètre, calcul d'incertitudes, validation de systèmes embarqués en cycle en V.

Je recherche un **stage de technicien de 10 semaines minimum dès avril 2027**, ou une **alternance pour ma 3e année de BUT dès septembre 2027**, en électronique, systèmes embarqués ou automatisme.

Formation
======
* **sept. 2025 – présent** · BUT Génie Électrique et Informatique Industrielle, Université de Toulouse
  * Parcours Électronique et Systèmes Embarqués : conception, programmation, automatisme, instrumentation, réseaux industriels. Diplôme prévu en juin 2028.
  * Chaîne de mesure : incertitudes de type A (répétabilité) et de type B (tolérances, résolution des CAN/CNA).
  * Habilitation électrique (1re année) ; maintenance (2e année) : AMDEC, analyse des défaillances, fiabilité et sécurité des systèmes.
* **juin 2025** · Baccalauréat général, spécialités Mathématiques et NSI, Lycée Saint-Sernin, Toulouse
* **juin 2022** · Brevet d'Initiation Aéronautique (BIA), Académie de Toulouse
* **2022** · Premiers secours civiques de niveau 1 (PSC1)

Expériences
======

* **2022** · Stage de découverte de 3e, ISAE-SUPAERO, Toulouse
  * Stage d'observation en ingénierie aéronautique, en complément du BIA : FabLab, simulateurs de vol et aérodrome.
* **oct. 2023 – présent** · Club Espace, [Le FabRiquet](https://fabriquet.fab-manager.com/#!/), Ramonville-Saint-Agne
  * Conception et impression 3D (Fusion 360) pour un projet de mini-fusée mené avec un club de passionnés.
  * Campagnes de lancements.
* **févr. 2025 – juin 2026** · Accompagnant éducatif bénévole, AFEV, Toulouse
  * Mentorat hebdomadaire (2 h) d'un élève de l'école primaire Alexandre Fourtanier ; engagement reconnu par l'Afev (« entière satisfaction »).
* **oct. 2026** · Lauréat 2026 du prix STEM for All, Paris
  * Prix Thales Solidarity, en partenariat avec l'Académie des technologies, pour encourager les vocations STEM d'étudiants méritants de 1re année.


Compétences
======
<div class="skills-wrapper">
    <ul class="skills-list">
        <li>
            <i class="fas fa-wave-square"></i>
            <span>Mesure et essais</span>
            <ul class="sub-skills">
                <li>Oscilloscope, multimètre, GBF et appareils de mesure électrique</li>
                <li>Tests et validation de systèmes électroniques, recherche de panne</li>
                <li>Calcul d'incertitudes (type A et B)</li>
                <li>Lecture de schémas électriques et de datasheets, soudure électronique</li>
            </ul>
        </li>
        <li>
            <i class="fas fa-microchip"></i>
            <span>Électronique et embarqué</span>
            <ul class="sub-skills">
                <li>Électronique de puissance</li>
                <li>Capteurs, PWM, commande moteur, Bluetooth</li>
                <li>GPIO, I2C, SPI, UART</li>
                <li>ESP32, STM32, Raspberry Pi</li>
            </ul>
        </li>
        <li>
            <i class="fas fa-robot"></i>
            <span>Automatisme</span>
            <ul class="sub-skills">
                <li>Automates programmables (API)</li>
                <li>TIA Portal (Siemens)</li>
                <li>Control Expert (Schneider Electric)</li>
            </ul>
        </li>
        <li>
            <i class="fas fa-code"></i>
            <span>Logiciels</span>
            <ul class="sub-skills">
                <li>C++, Python</li>
                <li>KiCad, Proteus, MATLAB</li>
                <li>Fusion 360, PlatformIO</li>
                <li>Microsoft Office</li>
            </ul>
        </li>
    </ul>
</div>

<style>
    .skills-wrapper {
        padding-left: 40px;
    }

    .skills-list, .sub-skills {
        list-style-type: none;
        padding-left: 0;
    }

    .skills-list > li {
        font-size: 16px;
        font-weight: 600;
        margin-bottom: 0.5rem; 
        display: flex;
        align-items: center;
        flex-wrap: wrap;
    }

    .skills-list > li > i {
        font-size: 1rem;
        color: #333;
        margin-right: 0.75rem;
        width: 20px;
        text-align: center;
    }

    .sub-skills {
        width: 100%;
        margin-top: 0.5rem;
        padding-left: 45px;
    }

    .sub-skills li {
        font-size: 13px;
        font-weight: 400;
        margin-bottom: 0.15rem;
    }

</style>


Projets
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
Loisirs
======
  <ul>{% for post in site.talks reversed %}
    {% include archive-single-talk-cv.html  %}
  {% endfor %}</ul>
  
Langues et loisirs
======
* **Langues** : français (langue maternelle), anglais B2, espagnol A2
* **Loisirs** : musique (guitare), basketball, voyage (vélo, randonnée, nature)
