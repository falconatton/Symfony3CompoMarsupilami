# Symfony3CompoMarsupilami
Création d'un carnet d'adresse pour Mr Marsupilami sous symfony 3.4


Travail sous Windows 10 systeme x64


objectif : créer un carnet d'adresse pour marsupilami sous symfony:
-Inscription/Connexion/Déconnexion du marsupilami par via login & mot de passe (FOSUserbundle)
-Afficher/Modifier ses informations : age / famille / race / nourriture...(Formulaire)
-Ajout/Suppression des marsupilamis de sa liste d'amis (relation "many to many" sur une seule table)
Toute initiative destinée à pimenter la vie des Marsupilami est la bienvenue.


1-Mise en place de l'envoronnement de travail





2-Inscription/Connexion/Déconnexion du marsupilami par via login & mot de passe (FOSUserbundle)

La quasi totalité des projets nécessitent une gestion des utilisateurs, ce bundle fais gagner du temps notamment d’un projet à un autre. Il permet  également l’utilisation d’autres bundles qui ont été pensé pour utiliser FOSUser.
FOSUserBundle : gère lui-même la connexion et l’inscription, c’est-à-dire qu’il va proposer un formulaire de base, 
mais aussi persister les données de l’utilisateur en base, le tout de manière sécurisée.

Astuce : Ne pas utiliser le "username" et le remplacer par le "mail".
Cela permet de recharger les droits automatiquement lors d’un ajout/retrait de rôle = cela évite de demander à l’utilisateur de se reconnecter!





Installation is a 7 step process:

-Download FOSUserBundle using composer

$ composer require friendsofsymfony/user-bundle "~2.0"

-Enable the Bundle
-Create your User class
-Configure your application's security.yml
-Configure the FOSUserBundle
-Import FOSUserBundle routing
-Update your database schema


