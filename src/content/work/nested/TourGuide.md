---
title: TourGuide
publishDate: 2026-03-16 00:00:00
img: /assets/tourguide.png
img_alt: Logo de l'application TourGuide
img_layout: logo
description: |
  Comparaison de deux modèles de concurrence pour optimiser une application touristique : CompletableFuture avec pool fixe et Virtual Threads Java 21.
tags:
  - Java
  - Spring Boot
  - API REST
  - CompletableFuture
  - Virtual Threads
  - JUnit
---

## Objectifs

Faire évoluer une application touristique capable de localiser les utilisateurs, proposer les attractions proches, calculer des récompenses et fournir des offres de voyage personnalisées.

## Réalisations

- calcul des cinq attractions les plus proches ;
- suivi de la position des utilisateurs ;
- calcul des points de récompense ;
- génération d'offres de voyage adaptées aux préférences ;
- traitement asynchrone avec `CompletableFuture` et pool de threads ;
- seconde implémentation basée sur les Virtual Threads de Java 21 ;
- tests fonctionnels et tests de performance à haut volume.

## Comparaison des modèles de concurrence

Le dépôt propose deux implémentations du traitement concurrent afin de comparer les approches sur les mêmes fonctionnalités métier et les mêmes scénarios de charge.

### Branche `master`

- Java 17 ;
- `CompletableFuture` pour lancer les traitements asynchrones ;
- pool fixe de 100 threads avec `Executors.newFixedThreadPool(100)` ;
- synchronisation globale avec `CompletableFuture.allOf(...).join()`.

### Branche `virtual-threads`

- Java 21 ;
- un Virtual Thread par tâche avec `Executors.newVirtualThreadPerTaskExecutor()` ;
- création de tâches génériques pour le suivi des positions et le calcul des récompenses ;
- attente de la fin des traitements avec `invokeAll` et `Future`.

Les tests de performance exécutent les deux stratégies sur les mêmes opérations : suivi de la position de plusieurs milliers d'utilisateurs et calcul concurrent de leurs récompenses. Cette organisation permet d'observer les différences de lisibilité, de gestion des ressources et de montée en charge entre threads de plateforme et Virtual Threads.

## Technologies utilisées

- Java 17 et Java 21
- Spring Boot 3
- Spring Web et Spring Validation
- CompletableFuture, ExecutorService et Virtual Threads
- JUnit 5
- APIs GPS Util, Reward Central et Trip Pricer

Liens GitHub :

- [Implémentation CompletableFuture](https://github.com/Guillaume-S92/TourGuideP8/tree/master)
- [Implémentation Virtual Threads](https://github.com/Guillaume-S92/TourGuideP8/tree/virtual-threads)
