### JWT -> Json Web Token 

- Header -> Infos du token 
- Informations de l'utilisateurs (INFOS)
- Date d'expiration (EXP)
- Signature
- Identifiant unique (SUB) -> Lien avec la BDD

**jwt.io pour se renseigner sur les tokens**

Génération d'un secret sur terminal : openssl rand -base64 45
## Etapes :

0. Stockage du secret ( clé de signature ) A mettre dans le fichier properties 
1. Gestion de l'autorisation 
2. Gestion de l'authentification 
3. Gestion du premier niveau d'interaction 
4. Implémentation de la logique métier? 