# projet-memoire-sdn

# README - Déploiement de la Topologie Réseau avec OpenDayLight

Ce projet vise à déployer une architecture réseau basée sur OpenDayLight (ODL) dans le cadre d'un système de Software-Defined Networking (SDN). Ce README fournit des instructions détaillées sur la mise en place de la topologie réseau décrite dans le Chapitre 3 du document.

## Introduction

OpenDaylight est un contrôleur SDN open-source développé par l'Open Networking Foundation (ONF) en collaboration avec divers acteurs de l'industrie. Il offre des fonctionnalités avancées de gestion de réseau, est entièrement basé sur Java, et dispose d'une interface graphique web (DLUX) pour surveiller et administrer le réseau.

## Matériels et Mise en Place du Système

### 3.1 Matériels

Dans cette section, nous détaillons les composants matériels utilisés pour mettre en place notre architecture SDN avec OpenDaylight. Nous utilisons :

- Une machine virtuelle Mininet déployée sur VMWare.
- Un switch Ethernet virtuel déployé sur GNS3.
- Une machine virtuelle Linux conteneurisée avec Docker, déployée sur GNS3 pour héberger le contrôleur OpenDayLight.
- Une machine virtuelle Linux avec Firefox utilisant Qemu, déployée sur GNS3 pour la gestion graphique du contrôleur OpenDayLight.

La topologie du réseau sur GNS3 est représentée dans la Figure 3.2 du document.

### 3.2 Mise en Place de l'Architecture

#### 3.2.1 Préparation de l'Environnement de Travail

- Ce projet est réalisé sous :
  - Emulateur GNS3 Version 2.2.31
  - VMWare Workstation 16 Pro

#### 3.2.2 Equipements Utilisés

Les équipements utilisés sont décrits précédemment dans la section "Matériels".

### 3.3 Déploiement de la Solution OpenDayLight pour l'Architecture SDN

Pour déployer OpenDayLight :

1. Téléchargez la version Carbon (0.6.4) à partir du lien https://docs.opendaylight.org/en/latest/downloads.html.
2. Décompressez le fichier téléchargé.
3. Lancez OpenDayLight en exécutant le script karaf.sh depuis le dossier bin via la ligne de commande.
4. Connectez-vous à l'interface d'administration de OpenDayLight à l'adresse https://ip-server-controller:8181/index.html en utilisant les identifiants par défaut (admin/admin).

### Guide de Déploiement de la Topologie Réseau avec OpenDayLight sur GNS3

Ce guide détaille les étapes pour déployer la topologie réseau décrite dans votre projet sur GNS3, en utilisant VMware pour héberger Mininet et une machine virtuelle GNS3 pour contrôler la topologie via OpenDayLight.

### Prérequis

Avant de commencer, assurez-vous d'avoir installé les logiciels suivants :

- GNS3 : Version 2.2.31 ou ultérieure.
- VMware Workstation : Pour héberger la machine virtuelle Mininet.
- VirtualBox (ou VMware Player) : Pour héberger la machine virtuelle GNS3.

### Étapes du Déploiement

#### 1. Importation du Projet dans GNS3

1. Lancez GNS3 et assurez-vous que VMware Workstation est configuré comme hyperviseur dans les préférences.
2. Importez le projet GNS3 que vous avez exporté. Assurez-vous que tous les fichiers sont correctement chargés.

#### 2. Configuration de la Machine Virtuelle Mininet

1. Ouvrez VMware Workstation et importez la machine virtuelle Mininet fournie avec le projet.
2. Configurez les paramètres réseau de la machine virtuelle Mininet pour qu'elle soit connectée au réseau virtuel de GNS3.

#### 3. Configuration de la Machine Virtuelle GNS3

1. Importez la machine virtuelle GNS3 fournie avec le projet dans VirtualBox ou VMware Player.
2. Assurez-vous que la machine virtuelle GNS3 est correctement configurée pour se connecter au réseau de GNS3 et à Internet.

#### 4. Lancement de la Topologie

1. Démarrez la machine virtuelle GNS3.
2. Ouvrez GNS3 et lancez la topologie importée.
3. Démarrez la machine virtuelle Mininet depuis VMware Workstation.
4. Assurez-vous que toutes les connexions entre les appareils dans la topologie sont établies et fonctionnelles.

#### 5. Configuration et Administration avec OpenDayLight

1. Démarrez le contrôleur OpenDayLight sur la machine virtuelle GNS3.
2. Accédez à l'interface d'administration de OpenDayLight via un navigateur web en utilisant l'adresse IP de la machine virtuelle GNS3.
3. Configurez et administrez la topologie réseau à l'aide de l'interface OpenDayLight.

### Conclusion

Ce guide fournit les étapes de base pour déployer la topologie réseau avec OpenDayLight sur GNS3. Assurez-vous de suivre attentivement chaque étape pour garantir un déploiement réussi de la topologie. En cas de problème, référez-vous à la documentation fournie avec votre projet pour des instructions spécifiques.

### 3.4 Discussion

La section "Discussion" présente une analyse des résultats et des perspectives futures du projet.

## Conclusion

Ce README fournit un aperçu des étapes nécessaires pour déployer la topologie réseau décrite dans le Chapitre 3 du document. Pour plus de détails, veuillez consulter le document complet.

