---
title: "Projet CHAINE DE PRODUCTION"
collection: publications
category: manuscripts
permalink: /publication/2026-06-01-paper-title-number-4
excerpt: 'Cette page présente la station AlgoPrime : un automate qui trie des pièces recyclables sur une chaîne de production.'
date: 2026-06-01
membres: 'Paguiel Nganji, <a href="https://www.linkedin.com/in/shahin-almostafa-495a553b0/">Shahin Almostafa</a>'
paperurl: 'https://paguielng.github.io/mdb2/files/cahier-de-labo-chaine-de-production.pdf'
citation: 'SAE Chaîne de production, BUT GEII, 2025-2026, avec Shahin Almostafa.'
---

{% include base_path %}

<div class="fiche" markdown="1">
**Cadre** : SAE Automatisme et informatique industrielle, BUT GEII, 2025-2026<br>
**Équipe** : binôme avec [Shahin Almostafa](https://www.linkedin.com/in/shahin-almostafa-495a553b0/)<br>
**Outils** : automate Schneider Modicon M340, Control Expert, GRAFCET, langage Ladder
</div>

## Le projet

<div class="activite-bloc">
<div class="activite-texte" markdown="1">
L'entreprise fictive AlgoGreen recycle des déchets sur une ligne automatisée. Avec Shahin, nous avons programmé la première station, **AlgoPrime**.

Elle trie les pièces qui arrivent sur le tapis : les pièces plates (recyclables) partent vers la station suivante, les pièces trouées continuent vers le four d'incinération.
</div>
<figure class="activite-image">
  <img src="{{ base_path }}/images/projets/chaine-de-production/station-algoprime.jpg" alt="La station AlgoPrime en salle de TP, avec son tapis et son bras manipulateur">
  <figcaption>La station AlgoPrime en salle de TP</figcaption>
</figure>
</div>

## Ce que nous avons fait

<div class="activite-bloc">
<div class="activite-texte" markdown="1">
Nous avons configuré l'automate M340 sous Control Expert, puis relié chaque capteur et chaque actionneur à son adresse d'entrée ou de sortie.

Nous avons ensuite décrit le cycle en **GRAFCET** et l'avons codé en **Ladder**. Deux palpeurs testent la pièce : si elle est plate, le bras la saisit par aspiration et la dépose dans l'ascenseur ; si elle est trouée, elle continue son chemin sans mobiliser le bras.
</div>
<figure class="activite-image">
  <img src="{{ base_path }}/images/projets/chaine-de-production/automate-m340.jpg" alt="Automate Schneider M340 câblé, avec ses cartes d'entrées et de sorties">
  <figcaption>L'automate M340 câblé</figcaption>
</figure>
</div>

<div class="activite-photos schemas">
  <figure>
    <img src="{{ base_path }}/images/projets/chaine-de-production/schema-pick-and-place.jpg" alt="Schéma du convoyeur, des palpeurs et du bras manipulateur">
    <figcaption>Capteurs et actionneurs de la station</figcaption>
  </figure>
  <figure>
    <img src="{{ base_path }}/images/projets/chaine-de-production/grafcet.jpg" alt="GRAFCET de la station avec ses deux chemins, pièce plate et pièce trouée">
    <figcaption>Notre GRAFCET : pièce plate à gauche, trouée à droite</figcaption>
  </figure>
</div>

Problème rencontré : le palpeur vertical et le bras restaient bloqués, car la même sortie était écrite à plusieurs endroits du programme et la dernière ligne l'emportait. Nous avons gardé une seule bobine par actionneur, avec toutes ses conditions en parallèle.
{: .notice}

## Ce que j'en retiens

Ce projet m'a fait passer de la théorie du GRAFCET à une vraie station : lire un cycle machine, adresser des entrées et sorties, et chercher la cause d'un défaut avec rigueur. Pour aller plus loin, nous aurions aimé ajouter une IHM sous Vijeo Designer et des compteurs de production.

<p><a class="btn btn--primary" href="{{ base_path }}/files/cahier-de-labo-chaine-de-production.pdf">Lire le cahier de laboratoire (PDF)</a></p>

{% include style-blocs.html %}
