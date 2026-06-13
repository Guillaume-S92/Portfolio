---
title: Heme Biotech Analytics
publishDate: 2024-03-15 00:00:00
img: /assets/heme-biotech.jpg
img_alt: Illustration Java pour le projet Heme Biotech Analytics
description: |
  Refactorisation d'une application Java d'analyse de symptômes avec comptage des occurrences, tri alphabétique et séparation claire des responsabilités.
tags:
  - Java
  - POO
  - Collections
  - Fichiers
---

## Objectifs

Reprendre une application Java existante afin de corriger son calcul des symptômes, améliorer sa maintenabilité et produire un fichier de résultats trié par ordre alphabétique.

## Réalisations

- lecture d'un fichier texte contenant les symptômes ;
- comptage dynamique des occurrences avec les collections Java ;
- tri des résultats avec une `TreeMap` ;
- écriture du résultat dans un fichier `result.out` ;
- séparation de la lecture, du traitement et de l'écriture grâce à des interfaces dédiées.

## Technologies utilisées

- Java
- programmation orientée objet
- `List`, `Map`, `HashMap` et `TreeMap`
- lecture et écriture de fichiers

Lien GitHub : [Heme Biotech Analytics](https://github.com/Guillaume-S92/heme-biotech-analytics)
