# Sprint 1

## En tant que visiteur, je veux visualiser les derniers biens en vente afin de découvrir les nouveautés de l'agence

Crée une entité user :

> symfony console make:user

- id
- nom
- mail
- password
- logo
- role

Crée une entité bien :

> symfony console make:entity

- adresse
- prix
- en_vente
- details
- images

Crée la page d'acceuil :

> symfony console make:controller

- modifier le controller pour envoyer les derniers bien en vente a la vue
- modifier la vue pour afficher les bien sous forme de carte
- crée un fichier vue pour un header de page
- la route est (/), on la nomme "home"

## En tant que visiteur, je veux visualiser les détails d'un bien afin de le découvrir

Crée une page pour visualiser un bien :

> symfony console make:controller

- modifier le controller pour envoyer le bien a la vue
- modifier la vue pour afficher le bien et ses details
- la route est (/bien/{id}), on la nomme "bien_view"

## En tant que visiteur, je veux contacter le conseiller en charge d'un bien afin de lui demander des précisions

Modifier la page bien_view :

- Crée un lien en base de donnée entre l'entité bien et user
- Modifier le controlleur pour qu'il envois aussi le vendeurs
- Ajouter une section dans la description pour avoir les informations sur le vendeur
