---
title: Le Vestiaire
publishDate: 2023-05-04 00:00:00
img: /assets/Le_Vestiaire.jpg
img_alt: image du site de vente de vétements Le Vestiaire
description: |
  Développement d'un site e-commerce basé sur les ventes de vétements.
tags:
  - Node
  - Express
  - MongoDB
  - React
  - Axios
  - Redux
---
## Objectifs

Création pour un projet personnel d'un site e-commerce spécialisé dans la vente de vétements. L'objectif est de pouvoir ajouter des articles aux paniers, modifié la quantité (ainsi que l'affiche du prix) et passer commande afin que cette dernière apparaisse dans la base de donnée avec un retour de confirmation de cette commande.

Création un site e-commerce dédié à la vente de vêtements dans le cadre d'un projet personnel. L'objectif principal est de permettre aux utilisateurs d'ajouter des articles à leur panier, de modifier les quantités (avec mise à jour automatique de l'affichage du prix) et de finaliser leur commande. Une fois la commande passée, celle-ci doit être enregistrée dans la base de données, et un retour de confirmation doit être généré pour l'utilisateur.

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

Il suffit de créer un fichier .env dans le dossier backend et d'ajouter ces valeurs avec les informations de votre Base de donnée MongoDB ainsi que la clée JWT et le port voulut :

MONGO_URL="mongodb+srv://username:password@cluster.mongodb.net/le_vestiaire"

PORT = "3001"

4 - Lancer le backend

cd server

npm start

5 - Lancer le frontend

cd frontend

npm start

##### Résultat

![image du du panier du site e_commerce Le Vestiaire](/assets/Le_Vestiaire_cart.jpg )
![image du la validation du produit e_commerce Le Vestiaire](/assets/Le_Vestiaire_validation.jpg)
![image de la validation des informations personnelles e_commerce Le Vestiaire](/assets/Le_Vestiaire_validation_adresse.jpg)
![image de la confirmation d'achat du site e_commerce Le Vestiaire](/assets/Le_Vestiaire_confirmation.jpg)

Lien github:  https://github.com/Guillaume-S92/mern-ecommerce-Le_Vestiaire.git