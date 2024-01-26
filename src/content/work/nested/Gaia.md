---
title: Gaia
publishDate: 2022-11-04 00:00:00
img: /assets/Gaia_presentation.jpg
img_alt: image du réseau social Gaia
description: |
  Développement d'un réseau social pour les passionnés de nature.
tags:
  - Node
  - Express
  - MySQL
  - React
  - Axios
  - Sass
---
## Objectifs

Création d'une API REST CRUD en tant que réseau social avec une interface plus agréable visualement et une possibilité d'ajout et de suppression de commentaire sous les posts.

## Technologies utilisées

- Backend (serveur) :
    * Express
    * Node
    * Javascript 
    * Base de données MongoDB

- Frontend (client):
    - React
    - Axios
    - Redux

##### Installation de l'application

1 - Installer le backend

cd server

npm install

2 - Installer le frontend

cd client

npm install

3 - Création de la base de données

Il suffit de créer un fichier .env dans le dossier server et d'ajouter ces valeurs avec les informations de votre Base de donnée MongoDB ainsi que la clée JWT et le port voulut :

MONGO_URL="mongodb+srv://username:password@cluster.mongodb.net/Gaia"

JWT_SECRET="codesecretsuperintrouvable"

PORT = "3001"

4 - Lancer le backend

cd server

npm start

5 - Lancer le frontend

cd frontend

npm start

##### Résultat

![image du Réseau social Gaia](/assets/Gaia.jpg )

Lien github:  https://github.com/Guillaume-S92/Gaia.git