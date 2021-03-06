---
layout: default
title: Travailler sur ordinateur à l'ENIT
parent: Services numériques
nav_order: 6
---

## Travailler sur ordinateur à l'ENIT
L’ENIT dispose de 5 salles « Informatique » équipées de postes permettant de travailler sur des machines virtuelles, disposant des logiciels nécessaires aux enseignements ayant lieu dans ces salles. Les documents et fichiers que vous manipulez et créez sur ces machines virtuelles sont stockés dans votre dossier personnel. Les salles info1 à info4 sont accessibles (accès par carte) lorsqu’il n’y a pas d’enseignement qui s’y déroule (voir EDT des salles sur planning.enit.fr et des salles info sur la porte d’info1).  
Ces mêmes machines virtuelles sont accessibles depuis les postes de la bibliothèque et depuis votre propre ordinateur si vous êtes sur le réseau de l’ENIT (voir ci-dessous).  
L’ENIT dispose aussi de 7 salles de bureau d’études, équipées de PC.  
Enfin, l’ENIT propose à ses étudiants et à son personnel un service de stockage et de partage de fichiers locaux et en ligne (un cloud).

### Wi-Fi
Pour connecter votre ordinateur sur le réseau wifi de l’ENIT, choisissez dans la liste des réseaux wifi disponibles le réseau ENIT. Saisissez votre identifiant LDAP pnom et le mot de passe associé pour terminer la connexion. Ce réseau est normalement enregistré et vous vous y reconnecterez automatiquement.

### VPN
Un VPN (Virtual Private Network) est un système permettant de créer un lien direct entre des ordinateurs distants, en isolant ce trafic. Cela permet de faire croire aux serveurs de l’ENIT que vous êtes sur place alors que vous travaillez chez vous.</p> Différents services « internes » à l’ENIT sont alors accessibles (ressources documentaires, machines virtuelles, serveurs de stockage, etc.).  
Pour installer le VPN de l’ENIT, allez à l’adresse [https://vpn.enit.fr](https://vpn.enit.fr)
- S’authentifier (LDAP),
- Télécharger la version correspondant à votre ordinateur
- Installer
- Lancer l’application installée.
- Indiquer le portail VPN de l’ENIT (vpn.enit.fr) puis vos identifiants
- Se connecter !
Vous êtes maintenant connectés comme si vous étiez à l’ENIT.  
Le réseau de l’ENIT étant surveillé et soumis au respect de la charte informatique, il est vivement conseillé de vous déconnecter du VPN lorsque vous avez fini de travailler.

### Machines virtuelles
Pour utiliser les machines virtuelles des salles info et de la bibliothèque sur votre ordinateur, rendez-vous sur l’extranet, menu Services/Numérique et SI, partie réseau.
- Tout en bas de la page, télécharger la version de VMWare Horizon proposée.
- Installer VMWare Horizon.
- Une fois le logiciel installé, lancer l’application.
- Menu Fichier/Nouveau serveur
- Saisir l’adresse du serveur : broker.ad.enit.fr
- Cliquer sur "Se connecter"
- S’authentifier (LDAP)  
![VMWare](images/VMWare.PNG)  
Vous êtes maintenant face au même ordinateur qu'en salle info.

### Dossiers personnels
Il est possible d’accéder aux répertoires (Mes Documents et Bureau) de ces machines virtuelles depuis son propre ordinateur, sur le réseau de l’ENIT. Une fois connecté au serveur, ce répertoire apparaitra dans les répertoires disponibles à gauche de votre fenêtre.

#### Windows
- Double-Cliquer sur l'icône ci-contre (il se trouve sur votre bureau)
- Cliquer sur "Connecter un lecteur réseau"
- Saisir les informations suivantes :
  - Lecteur : Z 
  - Dossier :\\nas4.enit.fr\users\students\pnom<
- Cliquer sur Terminer  
![dossierwindows](images/dossierwindows.PNG)  

#### MacOS
- Ouvrir Finder
- Menu "Aller" / "Se Connecter" au serveur
- Dans la barre d'adresse, saisir : smb:\\nas4.enit.fr\user\students\pnom
- Cliquer sur + pour mémoriser le serveur
- Connexion  
![dossiermac](images/dossiermac.PNG)  

### Le nuage de l'ENIT
A l’adresse nextcloud.enit.fr, vous aurez accès, après authentification par votre LDAP pnom et le mot de passe associé, à un espace de stockage et de partage de fichiers locaux et en ligne (un cloud), limité à 10Go.  
Les fichiers stockés dans votre espace sur ce serveur peuvent être :
- Synchronisés dans un répertoire sur votre propre ordinateur
- Partagés avec d’autres étudiants ou enseignants
- Modifiés directement en ligne

#### Synchronisation Nextcloud/répertoire local
Cette synchronisation entre votre espace Nextcloud et un répertoire local sur votre ordinateur se fait grâce à une application à installer sur votre ordinateur.
- Sur la page d’accueil de nextcloud.enit.fr, aller sur votre compte et sélectionner "Paramètres"  
![nextcloud](images/nextcloud.PNG)  
- Parmi les différentes configurations possibles, aller sur Mobile & bureau.
- Le bouton Desktop app vous amènera sur le site de téléchargement de l'application.  
![nextcloud2](images/nextcloud2.PNG)  
Lors de l'installation, deux choses à configurer :
- Le serveur à synchroniser est nextcloud.enit.fr, accès par votre compte LDAP (pnom et mot de passe associé),
- Le répertoire local à synchroniser, que vous mettez où vous voulez sur votre ordinateur individuel.

#### Partage
Il est possible de partager des fichiers ou des répertoires avec d’autres utilisateurs de Nextcloud. Ces fichiers ou répertoires seront automatiquement ajoutés à l’espace Nextcloud de la personne avec qui vous les partagez. Suivant vos choix de partage, cette personne pourra créer, modifier ou consulter les documents du partage. Les créations et modifications seront automatiquement reportées sur votre version des documents partagés.  
Pour partager un répertoire (ou un fichier) avec un ami depuis votre répertoire local :
- Aller dans le répertoire local Nextcloud
- Faire un clic droit sur le répertoire à partager
- Dans le menu contextuel, choisir "Share via Nextcloud" / "Share options"
- Dans la fenêtre de partage, taper le prénom et le nom de l’ami : Nextcloud cherche dans ses utilisateurs ceux correspondants
- Une fois l’ami sélectionné, il apparaît dans la liste en dessous, où vous pouvez modifier les options de partage ou supprimer le partage.
Pour partager un répertoire (ou un fichier) depuis l'interface web de Nextcloud, il faut cliquer sur le bouton à droite du nom de répertoire ou du fichier.  
![partagenextcloud](images/partagenextcloud.PNG)  
Il n’est pas possible de partager un répertoire ou un fichier de cette manière avec des gens extérieurs à l’ENIT. Vous pouvez simplement envoyer un lien qui permettra de télécharger les documents.

#### Modification en ligne
Nextcloud permet d’éditer des documents et de les modifier directement depuis l’interface web. Cela permet de rédiger des documents à plusieurs simultanément (alors que travailler simultanément sur un document synchronisé sur les répertoires locaux créera des copies du document).  
Il suffit de cliquer sur le nom du fichier sur l’interface web de Nextcloud pour qu’il s’ouvre en ligne. Les différents utilisateurs en train de travailler sur le fichier apparaissent en bas, entourés d’une couleur utilisée dans le document pour surligner les modifications qu’ils apportent.  
Les modifications effectuées en ligne ne sont reportées dans les répertoires locaux que tardivement.

### Salles Bureau d'études (salles BE)
Les ordinateurs des salles BE ne sont pas soumis à une authentification individuelle. Les documents de travail que vous y laissez ne sont donc pas en sécurité (plagiat, suppression, détournement, modification, etc.). Vous avez la possibilité de sauvegarder ces documents sur un serveur qui n’est pas non plus soumis à authentification, donc pas sûr.

#### Pour sauvegarder vos documents de travail en salles BE, utilisez les moyens suivants :
- Votre espace Nextcloud
- Espace des machine virtuelles des salles info 
- Un support amovible (clé USB, disque dur portable)
L’utilisation de Nextcloud vous permettra de partager les répertoires de travail de différents TP avec votre binôme.  
L’utilisation d’un support amovible comporte des risques, car les ordinateurs de salles BE sont ouverts à tous et peuvent être infectés.
