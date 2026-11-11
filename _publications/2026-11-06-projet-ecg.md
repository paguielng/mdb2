---
title: "Projet ÉLECTROCARDIOGRAPHE (ECG)"
collection: publications
category: manuscripts
permalink: /publication/2026-11-06-projet-ecg
excerpt: "Cette page présente le prototype d'une carte qui mesure, amplifie et filtre le signal électrique du cœur."
date: 2026-11-06
membres: 'Paguiel Nganji, Anis Bensenouci'
paperurl: 'https://paguielng.github.io/mdb2/files/cahier-de-labo-ecg.pdf'
citation: 'SAE Électronique ECG, BUT GEII 2e année, 2026-2027, avec Anis Bensenouci.'
---

{% include base_path %}

<div class="fiche" markdown="1">
**Cadre** : SAÉ Électronique du semestre 3, BUT GEII, IUT de Toulouse, 2026-2027<br>
**Équipe** : binôme avec Anis Bensenouci, au sein d'une équipe de quatre (deux binômes)<br>
**Outils** : FilterPro, Proteus, KiCad, AOP MCP6002, oscilloscope Keysight
</div>

## Le projet

<div class="activite-bloc">
<div class="activite-texte" markdown="1">
À chaque battement, le cœur produit sur la peau une tension d'environ 1 mV, noyée dans les parasites, surtout celui du secteur à 50 Hz. Le cahier des charges demandait le prototype d'une carte qui amplifie ce signal 500 à 1 500 fois et le filtre pour l'afficher sur un oscilloscope.

Avec Anis, nous avons pris en charge la carte d'alimentation, le **filtre passe-bas** (150 Hz) et le **filtre réjecteur 50 Hz**. L'autre binôme a réalisé l'amplification.
</div>
<figure class="activite-image">
  <img src="{{ base_path }}/images/projets/ecg/cartes-assemblees.jpg" alt="Cartes de l'ECG assemblées : alimentation, passe-bas et réjecteur">
  <figcaption>Nos cartes assemblées avant le test</figcaption>
</figure>
</div>

## Ce que nous avons fait

<div class="activite-bloc">
<div class="activite-texte" markdown="1">
Pour chaque filtre, nous avons suivi le même chemin : calcul des composants, simulation sous **FilterPro** et **Proteus**, implantation sous **KiCad**, soudure sur plaque à pastilles, puis test unitaire à l'oscilloscope.

Le passe-bas est une structure de Rauch d'ordre 2 avec un gain de 2. Pour le réjecteur, nous avons choisi un **Twin-T** bootstrappé, plus sélectif que la structure de Rauch essayée d'abord.
</div>
<figure class="activite-image">
  <img src="{{ base_path }}/images/projets/ecg/schema-fonctionnel.jpg" alt="Schéma fonctionnel de l'ECG dessiné au tableau, de l'électrode jusqu'à l'oscilloscope">
  <figcaption>Le schéma fonctionnel de la chaîne de mesure</figcaption>
</figure>
</div>

<div class="activite-photos schemas">
  <figure>
    <img src="{{ base_path }}/images/projets/ecg/implantation-passe-bas.jpg" alt="Schéma d'implantation KiCad du filtre passe-bas">
    <figcaption>Implantation KiCad du passe-bas</figcaption>
  </figure>
  <figure>
    <img src="{{ base_path }}/images/projets/ecg/implantation-rejecteur.jpg" alt="Schéma d'implantation KiCad du filtre réjecteur 50 Hz">
    <figcaption>Implantation KiCad du réjecteur 50 Hz</figcaption>
  </figure>
</div>

## Le test sur cobaye

<div class="activite-bloc">
<div class="activite-texte" markdown="1">
Toute la chaîne a été testée sur un camarade volontaire. Les pics du cœur apparaissent nets et réguliers, espacés de 640 ms, soit environ **94 battements par minute**.

Le parasite à 50 Hz reste pourtant bien visible : notre réjecteur n'atténuait que de 1 dB au lieu des 26 dB prévus.
</div>
<figure class="activite-image">
  <img src="{{ base_path }}/images/projets/ecg/ecg-cobaye.jpg" alt="Capture d'oscilloscope de l'ECG du cobaye avec les pics R et le parasite à 50 Hz">
  <figcaption>L'ECG du cobaye à l'oscilloscope</figcaption>
</figure>
</div>

Problème rencontré : pour approcher les valeurs calculées, nous avions associé huit condensateurs en parallèle dans le Twin-T. Trop de soudures, un câblage non conforme et le creux à 50 Hz a disparu. Un seul condensateur par branche, avec des résistances ajustées, aurait été plus fiable.
{: .notice}

## Ce que j'en retiens

Ce projet m'a fait parcourir tout le cycle en V sur un vrai système, du calcul au test sur une personne. J'ai surtout appris à refaire les calculs avec les composants réellement utilisés, à tenir compte de leurs tolérances et à garder une implantation simple pour limiter les erreurs.

<p><a class="btn btn--primary" href="{{ base_path }}/files/cahier-de-labo-ecg.pdf">Lire le cahier de laboratoire (PDF)</a></p>

{% include style-blocs.html %}
