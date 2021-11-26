# Sprint 2

---

## En tant qu'administrateur je veux créer de nouveaux utilisateurs

ET

## En tant qu'administrateur, je veux attribuer un rôle à un utilisateur

Crée la page d'administration :

> symfony console make:controller

- utiliser le bundle easyadmin3 afin de crée des page CRUD facilements et rapidement

> composer require easycorp/easyadmin-bundle

- la route est (/admin), on la nomme "admin"

---

## En tant que vendeur, je veux choisir un mot de passe afin d'accéder à mon espace personnel

Crée le système de mail avec Mailer

> composer require symfony/mailer

Crée un service qui va contenir la methode d'envois de mail

Crée un systeme d'authentification avec

> symfony console make:auth

Crée un formulaire de changement de mot de passe

> symfony console make:form

Dans ChangePassType, mettre les champs suivant :

- Mot de passe
- Confirmation du mots de passe
- boutton submit

---

## En tant que visiteur, je veux faire une proposition afin d'acheter un bien

Crée un formulaire PropositionType avec

> symfony console make:form
> qui contiendra les champs suivant :

- nom (si non connecter )
- Message
- boutton submit

---

## En tant que vendeur, je veux consulter les propositions reçus pour mon bien afin de les étudier

Crée la page vendeur :

> symfony console make:controller

- modifier le controller pour envoyer les propositions a la vue
- modifier la vue pour afficher une liste des propositions , comme un dashboard
- la route est (/vendeur), on la nomme "vendeur"

---

## En tant que conseiller, je veux pouvoir me connecter à mon espace sécurisé

Crée la page conseiller :

> symfony console make:controller

- modifier le controller pour envoyer les propositions a la vue
- modifier la vue pour afficher une liste des propositions , comme un dashboard
- la route est (/conseiller), on la nomme "conseiller"
