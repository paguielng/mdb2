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
* Bachelor universitaire de technologie, Université de Toulouse (en cours)
* Baccalauréat - Mathématiques, Informatique et physique-chimie, Lycée St. Sernin, 2025
* Stage de 3ème en ingénierie aéronautique, ISAE SUPAERO, 2022
* BIA - Brevet d'Initiation Aéronautique, Collège Toulouse-Lautrec, 2022
* Premiers secours Civiques de niveau 1 (PSC1), 2022

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
            <span>C / C++/ Web Development</span>
            <!-- Sous-compétences pour C/C++ -->
            <ul class="sub-skills">
                <li>Object-Oriented Programming (OOP)</li>
                <li>Memory Management (Pointers)</li>
                <li>Low-Level Programming (Hardware)</li>
                <li>Responsive HTML, CSS and JS web pages.</li>
            </ul>
        </li>

        <!-- Compétence Principale 2 -->
        <li>
            <i class="fas fa-microchip"></i>
            <span>Electronics & Hardware</span>
            <ul class="sub-skills">
                <li>Arduino / ESP32</li>
                <li>Signal analysis (Oscilloscope)</li>
                <li>Schematic & PCB Design</li>
            </ul>
        </li>

        <!-- Compétence Principale 3 -->
        <li>
            <i class="fas fa-robot"></i>
            <span>Robotics & Automation</span>
            <ul class="sub-skills">
                <li>Motor & Servomotor Control</li>
                <li>Sensors (IMU, Ultrasound)</li>
            </ul>
        </li>
        
        <!-- Compétence Principale 4 (MISE À JOUR) -->
        <li>
            <i class="fab fa-python"></i>
            <span>Python</span>
            <!-- Sous-compétences pour Python -->
            <ul class="sub-skills">
                <li>Scripting & Automation</li>
                <li>Data Analysis (Matplotlib, NumPy)</li>
                <li>Serial Communication with Microcontrollers</li>
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

    .sub-skills li {
        font-size: 0.85rem;
        font-weight: 400;
        margin-bottom: 0.15rem;
    }

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
  
Languages
======
<ul><em>French (native), English (fluent)</em></ul>

Service and leadership
======
* Currently signed in to 43 different slack teams
