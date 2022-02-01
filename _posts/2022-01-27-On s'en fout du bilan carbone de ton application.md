---
layout: post
title: "Faire le bilan carbone d'une application"
description: "Quoi regarder, quoi mesurer, qu'est-ce qui compte ?"
category: 
tags: [écologie, greenIT]
---

Ces dernières années, les discussions sur l'impact écologique du numérique continuent d'affluer. Tout est dit et 
son contraire. Peut-on être écolo et avoir un smartphone ? Doit on vider sa boite mail ? Doit on arrêter de regarder
du streaming vidéo ? Faut-il continuer de miner du bitcoin ?

Pour vous faire une bonne idée, je vous suggère de vous référer au site [greenIt](https://www.greenit.fr/).

Je vais donc donner mon avis sur la question du bilan carbone d'une application logicielle. 

# Pourquoi se soucier de l'impact écologique de nos applications ?

En deux mots, aujourd'hui l'empreinte du numérique est mineure, et représente entre 5 et 10% de l'empreinte carbone
des Français et Françaises. Néanmoins la part du numérique augmente continuellement depuis 20 ans dans le bilan 
carbone. Il s'agirait donc de surveiller
à minima que l'empreinte carbone du numérique ne croisse pas plus vite que ne décroissent les autres secteurs de nos vies
(habitat, production agricole, déplacements, etc.).

Pour plus d'informations, la page wikipedia est objective : [Impact environnemental du numérique](https://fr.wikipedia.org/wiki/Impact_environnemental_du_num%C3%A9rique).

# Comment calculer l'empreinte carbone ?

L'approche naïve de l'empreinte de ton application, c'est de calculer la consommation électrique de l'application déployée sur les 
serveurs et sur les terminaux utilisateurs, de multiplier ça par l'empreinte carbone de l'électricité (par exemple en France
l'électricité est essentiellement décarbonée, c'est-à-dire que la production d'électricité ne génère pas de gaz à effet de serre **GES**).

Calculer l'ensemble des transports de données (téléchargement de l'appli, des pages web) et multiplier ça par l'empreinte
carbone moyenne du transport de données.

Calculer le stockage sur disque total de l'appli et multiplier ça par l'empreinte carbone moyenne du stockage de données.


# Pourquoi ce n'est pas suffisant ?

## empreinte carbone != empreinte écologique

L'empreinte carbone ça ne fait pas tout.
Si on regarde [les limites planétaires](https://fr.wikipedia.org/wiki/Limites_plan%C3%A9taires), le climat n'est qu'une des
neuf limites de notre écosystème qui régulent la biosphère. 

![Limites planétaires](/images/limites%20planétaires.png)

### L'électricité n'est pas la seule empreinte de votre logicielle

En même si on se concentre uniquement sur l'aspect climatique des limites planétaires, l'électricité n'est qu'une
faible partie (18,5% du mix énergétique mondial, [src](https://fr.wikipedia.org/wiki/Mix_%C3%A9nerg%C3%A9tique)).


![résultats étude GreenIT](/images/green_concept.png)

On voit qu'il faut parler d'équivalent CO2, mais aussi de quantité d'eau, d'énergie, et de ressources. Et attribuer
ces postes de dépense à la fabrication des terminaux, l'usage des terminaux, l'usage du datacenter, l'installation
des réseaux et et la gestion de la fin de vie électronique.

## Le gain sera marginal 

Si vous faites ça, vous allez mettre l'effort sur des détails, optimiser des algorithmes pour moins consommer
de CPU, compresser des données pour le transport, minifier du javascript, etc.

**Loi de Campbell** : plus un indicateur quantitatif est utilisé pour la prise de décision, plus il a de chances de fausser et corrompre le processus qu’il a pour objet de surveiller

Avec cette démarche, vous économiserez 5% de la conso d'électricité à l'année. **C'est toujours ça de pris mais ça nous sauvera pas.**

## Quelques ordres de grandeur : 

* La principale source d’impact se situe au niveau des terminaux, essentiellement sur la phase de fabrication 
 qui représente entre 30% et 60% des impacts selon les indicateurs, et de manière moins significative sur
 la phase d’utilisation qui représente entre 1 et 17% des impacts selon les indicateurs
 
* La partie datacenter/cloud est également significative et en moyenne, elle représente entre 30% et 45% des impacts
 environnementaux 


*source* : [Green concept innovation](http://www.greenconcept-innovation.fr/wp-content/uploads/2020/02/greenconcept_21022020.pdf)

# Adopter une vision globale de l'application logicielle

Ce qu'il faut faire, en fait, c'est prendre de la hauteur.

Ce qui définit une application logicielle c'est l'association:

* d’équipements permettant de stocker, manipuler, afficher des octets (serveurs,
terminaux utilisateurs, box ADSL, etc.) ;
* d’infrastructures qui hébergent et relient les équipements (réseaux opérateurs et
centres de données notamment) ;
* de plusieurs logiciels empilés les uns sur les autres, qui s’exécutent au-dessus des
équipements;
* d’autres services numériques tiers éventuels (apis, services)

**A celà il faudrait ajouter une perspective fonctionnelle. Si votre application permet la location de voiture ou l'
achat de billets d'avion, il est peu probable que ça serve à quoi que ce soit de diminuer l'impact carbone de votre application.**


# Pour résumer 

## Priorité 1 : assurer que votre service tourne sur des appareils reconditionnés et anciens.

Le matériel numérique étant de très loin la plus importante part d'un service numérique, la top priorité est de 
limiter la quantité de matériel. 

C'est à dire :         
* faire en sorte que son application puisse tourner chez le consommateur sur des vieilles machines, supporter les vieux OS pour les applications lourdes, supporter les vieux navigateurs pour les applications légères
* permettre aux utilisateurs de continuer d'utiliser leur machine le plus souvent possible, de les revendre d'occasion, etc.
* limiter le nombre de machines nécessaires aux utilisateurs
* ne pas développer de services nécessitant des machines spécifiques. Par exemple les applications de réalité virtuelle qui demandent des nouveaux casques tous les ans sont une abomination **totale**, et je parle pas des voitures automatiques.

## Priorité 2 :assurer que notre service tourne sur une infrastructure mutualisée, dans un pays avec une électricité décarbonée

C'est ce qui est le plus efficace en terme de consommation énergétique.

## Pour aller plus loin, le pas ultime

Y a très peu de chance que ton service sauve la planète, mais on peut quand même se demander ?

* Est-ce que ton service est néfaste à la société ? Est-ce que ton job est d'afficher de la pub que personne ne veut ? Ou est-ce que tu nous développes des smart contracts dans une blockchain ? 
* Remplace-t'il du travail manuel par du capital logiciel, dans ce cas là, quel impact ? 
* Ton service permet-il de faciliter le travail carbone d'un gros pollueur ?
* Ton service permet-il de traffiquer des capteurs de pollution ? [coucou Volkswagen](https://fr.wikipedia.org/wiki/Affaire_Volkswagen) 
* Ton service participe-t'il à la société de consommation ? Ton service sert-il à maximiser des ventes ?


Si tu réponds oui à l'une de ces questions, peut-être qu'il faudrait juste ne pas développer ce produit.

### Quelques ressources pour aller plus loin :

La conférence d'Arthur Keller – [Les défis de notre temps : caractérisation systémique et stratégie systémique](https://www.youtube.com/watch?v=FoCN8vFPMz4)

Le podcast de Tristan Nitot [l'Octet Vert](https://anchor.fm/tristan-nitot)

Green IT : https://www.greenit.fr/ 

The Shift Project, tendance Lean ICT : https://theshiftproject.org/lean-ict/


