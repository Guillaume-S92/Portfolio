---
title: Groupomania
publishDate: 2022-07-04 00:00:00
img: /assets/Groupomania.jpg
img_alt: image du réseau social Groupomania
description: |
  Développement d'un réseau social d'entreprise.
tags:
  - Node
  - Express
  - MySQL
  - React
  - Axios
  - Sass
---
## Objectifs

Création d'une API REST CRUD en tant que réseau social d'entreprise.

## Technologies utilisées

- Backend (serveur) :
    * Express
    * Node
    * Javascript 
    * Base de données MySQL

- Frontend (client):
    - Axios
    - React
    - Sass

##### Installation de l'application

1 - Installer le backend

cd backend

npm install

2 - Installer le frontend

cd frontend

npm install

3 - Création de la base de données

Connectez-vous à votre base de données en remplaçant le nom d'utilisateur mysql -u nom d'utilisateur -p

Saisissez votre mot de passe puis tapez sur la touche entrée

Créez une nouvelle base de données en remplaçant dbname par le nom de votre choix : CREATE DATABASE dbname

Puis rendez-vous dans le fichier database.js du back-end et modifier les valeurs suivantes :

let connection = mysql.createConnection({
host: 'localhost',
user: 'root',
password: '',
database: 'groupomania'
});

Remplacez : 'root' par votre 'nom d'utilisateur' indiquez entre '' votre mot de passe (si vous en avez mis un pour cet utilisateur) 'test' par le nom de la base de données que vous venez de créer (NOM_BDD)

Tapez la commande suivante :

mysql -u NOM_UTILISATEUR -p NOM_BDD < dump.sql

en remplaçant NOM_UTILISATEUR et NOM_BDD par ceux modifiés précédemment

6 - Lancer le backend

cd backend

nodemon server

7 - Lancer le frontend

cd frontend

npm run start

##### Résultat

Lien github:  https://github.com/Guillaume-S92/Groupomania-social-network--learn-javascript-back-and-front.git