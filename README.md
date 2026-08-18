# README

[![Release](https://img.shields.io/docker/v/jcpd/dknr-daikin?sort=semver)](https://img.shields.io/docker/v/jcpd/dknr-daikin?sort=semver)
[![Pull](https://img.shields.io/docker/pulls/jcpd/dknr-daikin)](https://img.shields.io/docker/pulls/jcpd/dknr-daikin)
[![Issue](https://img.shields.io/github/issues/jcdenis/dknr-daikin)](https://img.shields.io/github/issues/jcdenis/dknr-daikin)
[![License](https://img.shields.io/github/license/jcdenis/dknr-daikin)](https://github.com/JcDenis/dknr-daikin/blob/master/LICENSE)


## A propos

**dknr-daikin** est un projet consacré au pilotage, à la récupération et à l'exploitation des données des PAC Daikin en local. Ce projet n'utilise pas le cloud Daikin mais attaque directement l'API des unités Daikin.

[![Dashboard Screenshot detail](https://github.com/JcDenis/dknr-daikin/blob/master/sshot/dknr-daikin_screenshot.png)](https://github.com/JcDenis/dknr-daikin/blob/master/sshot/dknr-daikin_screenshot.png)

[![Dashboard Screenshot chart](https://github.com/JcDenis/dknr-daikin/blob/master/sshot/dknr-daikin_screenshot2.png)](https://github.com/JcDenis/dknr-daikin/blob/master/sshot/dknr-daikin_screenshot2.png)

[![Dashboard Screenshot add](https://github.com/JcDenis/dknr-daikin/blob/master/sshot/dknr-daikin_screenshot3.png)](https://github.com/JcDenis/dknr-daikin/blob/master/sshot/dknr-daikin_screenshot3.png)

[![Dashboard Screenshot mqtt](https://github.com/JcDenis/dknr-daikin/blob/master/sshot/dknr-daikin_screenshot4.png)](https://github.com/JcDenis/dknr-daikin/blob/master/sshot/dknr-daikin_screenshot4.png)


## Fonctionnalités

- **Support de plusieurs unités interieurs**.
- **Décodage des valeurs des unités interieurs** et extraction des valeurs utiles.
- **Exploitation locale des mesures** pour le suivi de la consommation.
- **Intégration possible** dans une installation domotique ou un outil de supervision.
- **Support Home-Assistant Discovery** en lecture et pilotage des unités.


## Matériel requis

Le matériel exact dépend de l'installation, mais l'utilisation du projet nécessite généralement :

* une ou plusieurs unites interieurs Daikin avec module Wifi/Ethernet.
* une machine exécutant le logiciel docker et connectée au même réseau que les unités.

Ce projet a été testé avec une unité équipée du module Wifi **BRP069Bxx** mais devrait supporter les modules suivants :

* BRP069Axx
* BRP069Bxx
* BRP069B4x
* BRP072Axx

D'autres modules peuvent être supportés, si vous en connaissez ils peuvent être ajouté à cette liste.


## Installation

Des images Docker prêtes à l'emploi sont disponibles. 
Utilisez le fichier docker-compose.yaml à la racine du dépôt en fournissant les variables d'environnement suivantes :

* **DKNR_USERNAME** : login de l'interface node-red.
* **DKNR_PASSWORD** : mot de passe de l'interface node-red.
* **DKNR_SECRET**   : un mot secret pour encrypter les credits.


## A faire

* **Mode découverte** pour rechercher automatiquement les appareils sur le réseau local.
* N'afficher que les options disponibles suivant le modèle.


## Contribuer

Ce projet est **open-source**, vous pouvez participer en créant des [tickets](https://github.com/JcDenis/dknr-daikin/issues) ou en proposant de [requêtes](https://github.com/JcDenis/dknr-daikin/pulls) sur le dépôt github du projet.


## Voir aussi

- [DKNR Teleinfo](https://github.com/JcDenis/dknr-teleinfo)
- [DKNR APSystems](https://github.com/JcDenis/dknr-apsystems)
- [DKNR Daikin](https://github.com/JcDenis/dknr-daikin)
