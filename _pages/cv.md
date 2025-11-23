---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
======
* Ph.D in Version Control Theory, GitHub University, 2018 (expected)
* M.S. in Jekyll, GitHub University, 2014
* B.S. in GitHub, GitHub University, 2012

Work experience
======
* Spring 2024: Academic Pages Collaborator
  * GitHub University
  * Duties includes: Updates and improvements to template
  * Supervisor: The Users

* Fall 2015: Research Assistant
  * GitHub University
  * Duties included: Merging pull requests
  * Supervisor: Professor Hub

* Summer 2015: Research Assistant
  * GitHub University
  * Duties included: Tagging issues
  * Supervisor: Professor Git
  
Skills
======
<div class="skills-wrapper">

    <ul class="skills-list">
        <!-- Compétence Principale 1 -->
        <li>
            <i class="fas fa-code"></i>
            <span>C / C++</span>
        </li>

        <!-- Compétence Principale 2 -->
        <li>
            <i class="fas fa-microchip"></i>
            <span>Électronique & Hardware</span>
            <ul class="sub-skills">
                <li>Arduino / ESP32</li>
                <li>Analyse de signaux (Oscilloscope)</li>
                <li>Conception de schémas & PCB</li>
            </ul>
        </li>

        <!-- Compétence Principale 3 -->
        <li>
            <i class="fas fa-robot"></i>
            <span>Robotique & Automatisme</span>
            <ul class="sub-skills">
                <li>Contrôle de moteurs & servomoteurs</li>
                <li>Capteurs (IMU, Ultrasons)</li>
            </ul>
        </li>
        
        <!-- Compétence Principale 4 -->
        <li>
            <i class="fab fa-python"></i>
            <span>Python</span>
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
        font-size: 1.2rem;
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

    /* LES MODIFICATIONS SONT ICI */
    .sub-skills li {
        font-size: 0.9rem;
        font-weight: 400;
        margin-bottom: 0.15rem;  /* Espace vertical encore plus réduit */
        /* J'ai enlevé 'position: relative' et 'padding-left' qui n'étaient utiles que pour la puce */
    }

    /* J'ai supprimé toute la règle '.sub-skills li::before' pour enlever les cercles */

</style>


Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
Talks
======
  <ul>{% for post in site.talks reversed %}
    {% include archive-single-talk-cv.html  %}
  {% endfor %}</ul>
  
Teaching
======
  <ul>{% for post in site.teaching reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
Service and leadership
======
* Currently signed in to 43 different slack teams
