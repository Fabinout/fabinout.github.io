---
layout: post
title: "Résumé formation GCP"
description: "notes formation SFEIR"
tags: [nada]
---

Formation GCP


## Introduction au Cloud

@DidierGirard

Le cloud n'est plus simplement un moyen d'hoster des applications, c'est maintenant une gigantesque boite à outil pour tout faire.
De l'IA, de la Data, de l'application.

La puissance de calcul des processeurs n'augmente plus autant qu'avant, l'avenir est au scale-out (déployer sur une autre machine) plutôt que le scale-up (déployer
sur une machine plus puissante). 

#### Cloud is cheaper
Ça dépend de ce qu'on fait

#### Cloud is flexible
C'est vrai

#### En tant qu'ingénieur, c'est dangereux de rester sur le on-prem

Le cloud est l'avenir (selon les dires de Sfeir ;) ), en tant qu'ingénieur, c'est intéressant de se pencher dessus comme on
se pencherait sur le nouveau langage à la mode. De plus y aura besoin de développeurs à la place de sys admin/devops.

### Comment choisir son cloud-provider

Chacun a ses spécificités : 
si vous êtes historiquement d'un système windows, c'est plus intéressant d'aller sur Azure
si vous cherchez une infrastructure qui fonctionne comme un datacenter, go Amazon (beaucoup de service permettant de manager à-la-datacenter)
si vous cherchez un cloud-provider avec des outils parfaitement adaptés au cloud, go GCP (ça demande de remettre en question la manière dont on fait de l'informatique) 

### Histoire de Google Cloud Platform

Un OPS chez google, ça administre 100 000 serveur, c'est fait pour aller très très loin dans l'automatisation.
Ils ont pris des développeurs pour l'administration de leur système, et ils ont automatisé ENORMÉMENT de tâches.

Google fait du crawling, de la data, du transport d'information (c'est leur coeur de métier), ils sont très forts sur ces
axes là, et aller sur GCP, c'est aussi louer leurs applications.

### Aller vers un cloud flexible

On estime qu'on est dans la troisième génération 

---------------
User-configured, managed and maintained

Gen 1 : Physical, on met l'IT sur des machines physiques, dans des batiments physiques
Gen 2 : Virtualized, on loue des VMs chez un provider, mais on travaille comme avant

------------------

Fully automated

Gen 3 : Serverless/Devops , on voit le cloud comme des services


### Google c'est aussi 

7 services avec plus d'1 milliard d'utilisateur, donc c'est les premiers consommateurs de leur service

### Nouvelle vitesse

Entre l'idée et le déploiement en prod scalé, un projet peut être fait maintenant en quelques semaines. Ça change pas mal de chose
notamment sur la croissance et sur l'innovation. 

# Les 7 services Cloud Computing

* Compute
* Network diffuser, communiquer
* Storage stocker de l'information, est-ce que je peux stocker des vidéos, des images
* Database (quels types de DB sont proposés)
* Analytics (quels outils, comment manipuler et analyser la donnée que j'ai récolé)
* IA 

#### Compute

Compute Engine (VM)
Kubernetes Engine (pour des conteneurs)
App engine
Functions

#### Network

CDN, CVN, DNS, etc.

#### Data

Pub sub (capter des data)
Data flow (transformer des data)
Big Query (stocker pour un datalake)

#### Machine Learning

Louer des outils qui font du ML (pleins que je connais pas)

## Une stratégie pour le cloud ?

On fait un POC en une semaine, on valide que ça marche

On fait un cloud Plan, on prépare la migration d'une VRAIE application sur le cloud (design document, application design, ddd, etc.)

## Structurer les projets

Une équipe a un projet, qui regroupe toutes ses ressources

* Org
* Folders
* Projets
* Ressources

Les droits et accès sont hérités de haut en bas.

C'est important de commencer par la structuration pour éviter que ça devienne trop vite le bordel.

### Gérer les identités et les accès

SSO, SAML2.0 et OPenID ouverts.

Cloud Identité pour gérer qui est qui
Cloud IAM pour gérer les droits alloués à tel ou tel ressource

#### Comment s'identifier

Google IDaaP  (gsuite user) you@domain.com
google account you@gmail.com
un compte de service you@project_id.iam.gserviceaccount.com

Un compte de service est un compte avec des droits, ça permet de faire les étapes d'automatisation. Ça permet à une machine
de manipuler l'infrastructure.

Bonne pratique : 
* on assigne des permissions à des groupes plutôt qu'à des individus

### Marketplace GCP

"J'aimerais avoir une bdd Cassandra" on peut aller dans la marketplace et avoir accès à ce software, sans avoir à le manager.

## GKE On-prem

on peut monter un cluster on-premise, managé par le GKE cloud, et qui déborde au besoin sur le cloud. Check Anthos  


