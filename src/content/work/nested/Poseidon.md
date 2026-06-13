---
title: Poseidon Capital Solutions
publishDate: 2026-01-01 00:00:00
img: /assets/Poseidon_Capital_Solutions.png
img_alt: Interface de gestion des offres de Poseidon Capital Solutions
img_layout: screenshot
description: |
  Application Spring Boot MVC de gestion de données financières avec CRUD, validation, authentification et autorisations par rôles.
tags:
  - Java
  - Spring Boot
  - Spring Security
  - Spring Data JPA
  - Thymeleaf
  - MySQL
---

## Objectifs

Finaliser le back-end d'une application interne de trading en implémentant les fonctionnalités métier, la validation des formulaires et la sécurité des accès.

## Réalisations

- opérations CRUD sur les offres, courbes, notations, règles, transactions et utilisateurs ;
- validation des données saisies dans les formulaires ;
- authentification par session et rôles `ADMIN` / `USER` ;
- chiffrement des mots de passe avec BCrypt ;
- tests unitaires des services et tests de sécurité.

## Technologies utilisées

- Java 17 et Spring Boot 3
- Spring Web, Spring Data JPA et Spring Security
- Thymeleaf et Bootstrap
- MySQL et H2
- Maven, JUnit, Mockito et Jasypt

![Liste des offres de Poseidon](/assets/poseidon-bids.png)
![Formulaire d'ajout d'un utilisateur](/assets/poseidon-add-user.png)

Lien GitHub : [Poseidon Capital Solutions](https://github.com/Guillaume-S92/P7_Poseidon-Capital-Solutions)
