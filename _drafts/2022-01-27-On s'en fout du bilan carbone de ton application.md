---
layout: post
title: "Faire le bilan carbone d'une application"
description: "On s'en fout"
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

Pour plus d'informations, la page wikipedia est objective : [Impact environnemental du numérique](https://fr.wikipedia.org/wiki/Impact_environnemental_du_num%C3%A9rique)

# Comment calculer l'empreinte carbone ?

L'approche naïve de l'empreinte de ton application, c'est de calculer la consommation électrique de l'application déployée sur les 
serveurs et sur les terminaux utilisateurs, de multiplier ça par l'empreinte carbone de l'électricité (par exemple en France
l'électricité est essentiellement décarbonée, c'est-à-dire que la production d'électricité ne génère pas de gaz à effet de serre **GES**).

Calculer l'ensemble des transports de données (téléchargement de l'appli, des pages web) et multiplier ça par l'empreinte
carbone moyenne du transport de données.

Calculer le stockage sur disque total de l'appli et multiplier ça par l'empreinte carbone moyenne du stockage de données.


# Pourquoi ce n'est pas suffisant ?


## le gain sera marginal 

Si vous faites ça, vous allez mettre l'effort sur des détails, optimiser des algorithmes pour moins consommer
de CPU, compresser des données pour le transport, minifier du javascript, etc.

     **Loi de Campbell** : plus un indicateur quantitatif est utilisé pour la prise de décision, plus il a de chances de fausser et corrompre le processus qu’il a pour objet de surveiller

Avec cette démarche, vous économiserez 5% de la conso d'électricité à l'année. **C'est toujours ça de pris mais ça nous sauvera pas.**

## empreinte carbone != empreinte écologique

L'empreinte carbone ça ne fait pas tout.
Si on regarde les limites planétaires 

![Limites planétaires](/images/limites%20planétaires.png)




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



[Arthur Keller – Les défis de notre temps : caractérisation systémique et stratégie systémique](https://www.youtube.com/watch?v=FoCN8vFPMz4)