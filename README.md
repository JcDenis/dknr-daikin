# README

[![Release](https://img.shields.io/docker/v/jcpd/dknr-daikin?color=lightblue)](https://hub.docker.com/r/jcpd/dknr-daikin)
[![License](https://img.shields.io/github/license/jcdenis/dknr-daikin?color=white)](https://github.com/JcDenis/dknr-daikin/blob/master/LICENSE)


## A propos

**dknr-daikin** est un projet consacré à la récupération et à l'exploitation des données des PAC Daikin en local.

[![Dashboard Screenshot](https://github.com/JcDenis/dknr-daikin/blob/master/dknr-daikin_screenshot.png)](https://github.com/JcDenis/dknr-daikin/blob/master/dknr-daikin_screenshot.png)


## Fonctionnalités

- **Support de plusieurs unités interieurs**.
- **Décodage des valeurs des unités interieurs** et extraction des valeurs utiles.
- **Exploitation locale des mesures** pour le suivi de la consommation.
- **Intégration possible** dans une installation domotique ou un outil de supervision.


## Matériel requis

Le matériel exact dépend de l'installation, mais l'utilisation du projet nécessite généralement :

* une ou lusieurs unites interieurs Daikin avec module Wifi/Ethernet.
* une machine exécutant le logiciel docker.


## Installation

Des images Docker prêtes à l'emploi sont disponibles. 
Utilisez le fichier docker-compose.yaml à la racine du dépôt en fournissant les variables d'environnement suivant :

* DKNR_USERNAME : login de l'interface node-red
* DKNR_PASSWORD : mot de passe de l'interface node-red
* DKNR_SECRET   : un mot secret pour encrypter les credits.
