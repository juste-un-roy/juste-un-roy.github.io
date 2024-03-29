---
layout: post
title: Python à la rescousse d'un bibliothécaire débordé
excerpt: "À la bibliothèque de l'École de Technologie supérieure, l'utilisation de Python a permis d'accélérer la classification de revues de la littérature."
modified: 24/09/2022, 17:37
tags: [analyse et fouille de texte, Python]
comments: true
category: blog
---

En été 2022,  l'équipe de l'École de Technologie Supérieure (ÉTS) a initié un projet bien particulier : repérer toutes les revues de la littérature (_review articles_) publiées par les chercheurs et chercheuses de l'École, puis les classer par type de revue de la littérature (systématique, état de l'art, etc.). En qualité d'étudiant intéressé par la recherche universitaire, c'est à moi qu'est incombé ce dossier.

Très vite, je me suis rendu compte que l'exercice nécessiterait de recourir à une intelligence artificielle : les notices de __630 articles__ demandaient à être scrutées! Procéder manuellement aurait pris des semaines, empiétant sur un temps susceptible d'être accordé à biens d'autres projets. Résolu à m'éviter un travail aussi répétitif que chronophage, j'ai programmé un algorithme capable d'automatiser une partie du processus de classification.

Notre méthode a révélé que le moteur de recherche de _Scopus_ était moins précis que celui de _Web of Science_ pour identifier des revues de la littérature. Elle a aussi montré que les types de revue de la littérature les plus fréquents, à l'ÉTS, sont les revues de la littérature au sens classique, les revues de la littérature systématique et les revues de la littérature du type « état de l'art ».

Ces résultats ont été présentés au personnel de la bibliothèque, de façon à faire valoir la pertinence des compétences technologiques en milieu universitaire. En effet, dans des équipes de petites tailles comme à l'ÉTS, l'automatisation de certaines tâches répétitives peut permettre aux bibliothécaires de se concentrer sur leurs relations avec la communauté universitaire ou sur des dossiers pressants.

### Méthodologie

L'[algorithme](https://github.com/juste-un-roy/FT-Classification-Automatique) a été codé en Python avec l'aide de Clara Turp, alors bibliothécaire système à l'Université McGill. Très simple, il procède en recherchant une liste d’expressions régulières dans la notice d’un article. L’occurrence et la fréquence de chaque expression dans la notice sont comptabilisées, de façon à faciliter sa classification manuelle a posteriori.

Nous avons traité la diversité et la fréquence des occurrences comme des indicateurs nous permettant de pondérer la catégorie d'un artile et la probalité qu'il soit réellement ou non une revue de la littérature. Cette méthode nous a permis d'identifer rapidement les faux positif au sein de notre corpus. 

### Corpus
Le corpus soumis à notre algorithme était un ensemble de 630 notices de revues de la littérature publiées par des chercheurs de l'ÉTS, téléchargées en format CSV sur les bases de données _Web of Science_ et _Scopus_. Cet ensemble de textes a été nettoyé et préparé pour l'expérimentation en utilisant _Open Refine_.
