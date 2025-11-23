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
* Skill 1
* Skill 2
  * Sub-skill 2.1
  * Sub-skill 2.2
  * Sub-skill 2.3
* Skill 3

    <section id="skills" class="container">
        <div class="skills-grid">
            <div class="skill-card"><i class="fas fa-code"></i> C / C++</div>
            <div class="skill-card"><i class="fas fa-microchip"></i> Arduino / ESP32</div>
            <div class="skill-card"><i class="fas fa-bolt"></i> Électronique Analogique & Numérique</div>
            <div class="skill-card"><i class="fas fa-wave-square"></i> Analyse de signaux (Oscilloscope)</div>
            <div class="skill-card"><i class="fas fa-cogs"></i> Automatisme</div>
            <div class="skill-card"><i class="fab fa-python"></i> Python (Notions)</div>
        </div>
    </section>
<style>
  .skills-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 20px;
    text-align: center;
}
</style>
<style>
.skill-card {
    background-color: var(--card-bg);
    padding: 20px;
    border-radius: 8px;
    box-shadow: 0 4px 8px rgba(0,0,0,0.05);
    font-size: 1.1rem;
}
</style>
<style>
.skill-card i {
    font-size: 2rem;
    color: var(--secondary-color);
    margin-bottom: 10px;
    display: block;
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
  
Service and leadership
======
* Currently signed in to 43 different slack teams
