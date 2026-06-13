---
title: Medilabo
publishDate: 2026-06-06 00:00:00
img: /assets/medilabo-login.png
img_alt: Écran de connexion de la plateforme médicale Medilabo
img_layout: screenshot
description: |
  Plateforme médicale en microservices avec API documentée par OpenAPI pour gérer les patients, les notes cliniques et le risque de diabète.
tags:
  - Java
  - Spring Boot
  - Microservices
  - OpenAPI
  - Swagger UI
  - Angular
  - Docker
  - MySQL
  - MongoDB
---

## Objectifs

Construire une plateforme sécurisée permettant au personnel médical de suivre les patients et de calculer leur niveau de risque de diabète à partir de leurs données et notes cliniques.

## Architecture

L'application est composée d'un front Angular, d'une gateway Spring Cloud et de quatre microservices :

- authentification et gestion des jetons JWT ;
- gestion des patients dans MySQL ;
- gestion des notes médicales dans MongoDB ;
- calcul du niveau de risque de diabète.

L'ensemble de la plateforme est orchestré avec Docker Compose.

## Documentation des API

Chaque microservice génère son propre contrat OpenAPI avec `springdoc-openapi`. La gateway rassemble ces contrats dans une interface Swagger UI centralisée permettant de parcourir et tester les API d'authentification, de gestion des patients, des notes médicales et d'évaluation des risques.

Les endpoints métier restent sécurisés par JWT. Swagger UI intègre un mécanisme d'autorisation permettant de transmettre le token Bearer lors des requêtes protégées.

Une fois l'application lancée, la documentation est accessible à l'adresse :

`http://localhost:8080/swagger-ui.html`

## Technologies utilisées

- Java 21, Spring Boot et Spring Cloud Gateway
- Spring Security, JWT et BCrypt
- OpenAPI, Swagger UI et springdoc-openapi
- Spring Data JPA, MySQL et MongoDB
- Angular et TypeScript
- Docker, Docker Compose et Nginx

![Connexion à Medilabo](/assets/medilabo-login.png)
![Liste des patients Medilabo](/assets/medilabo-patients.png)
![Évaluation du risque dans Medilabo](/assets/medilabo-assessment.png)

Lien GitHub : [Medilabo](https://github.com/Guillaume-S92/Project_9_Medilabo)
