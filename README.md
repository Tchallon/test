# Installation et configuration du site d'histeria

## Prérequis

* Une base de donnée MySql
* Un serveur possédant PhP 7.2 minimum

## Configuration des bases de données

> Se rendre dans le dossier : `/script/` depuis la racine du site
* Editer le fichier : `database.php` --> **Correspond à la base de donnée du site**
* Editer le fichier : `server_database.php` --> **Correspond à la base de donnée du serveur** *sera utilisé juste pour lire la table de la v5*
* Modifier les entrées de variables des deux fichiers tels que : 
> * host, par défault localhost cependant si utilisation base de donnée distante mettre le nom de domaine/ip pour y accéder
> * db_name, le nom de la base de donnée alloué au site web, ce sera là que les tables seront créer
> * user, le nom d'utilisateur pour accéder à la base de donnée
> * pass, le mot de passe pour accéder à la base de donnée

## Configuration du module RCON

> Se rendre dans le dossier : `/admin/` depuis la racine du site
* Editer le fichier : `index.php`
* Modifier les premières variables du fichier tels que :
> * server_adr, correspond à l'ip / host du serveur où les commandes seront envoyées
> * server_port, correspond au port de connexion du serveur
> * rcon_passwd, correspond au mot de passe pour envoyer les commandes rcon

Je te conseille dejà de rentrer les données d'un serveur de test et une fois la configuration terminé, revenir mettre les valeurs du vrai serveur.

## Installation de la base de donnée

**Veuiller avoir correctement effectué la partie de configuration de la base de donnée**
> Se rendre dans le dossier : `/init/` depuis la racine du site
* Y déposer le fichier `stats.csv` contenant la table de la v4.5
* Ouvrir sur le site web : `<nom de domaine>/init/main.php`
Si une anomalie est trouvé merci de me contacter

*Le site est automatiquement mit en maintenance une fois ce fichier ouvert*

*Pour la suprimer rend toi dans le panel admin dispo ici : `<nom de domaine>/admin/`*

Y rentrer les identifiants qu'on s'est envoyé sur discord
