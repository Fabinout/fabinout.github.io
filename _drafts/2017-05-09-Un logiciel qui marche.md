---
layout: post
title: "Un logiciel qui marche, l'allégorie industrielle"
description: "Logiciel travaillant au dessus d'une documentation compréhensible"
category: 
tags: [Clean Code, Agile]
---

Parlons un peu d'un des 4 piliers de l'agile. 

> Working software over comprensive documentation    

Pour clarifier tout de suite, ce pilier de l'agile **ne dit pas** qu'il ne faut pas rédiger 
de documentation. L'objectif de l'agile est de fournir de la meilleure manière possible 
un logiciel à des utilisateurs, et d'être capable de modifier son process régulièrement. 
Cet adage vise donc à reconcentrer les efforts des membres de l'équipe 
autour du produit final, **un logiciel qui marche**.    

Cet article se base sur ma lecture récente de **Le but : Un processus 
de progrès permanent** de Eliyahu Goldratt : [Lien amazon](https://www.amazon.fr/but-processus-progr%C3%A8s-permanent/dp/2124654047).   
Je vous conseille chaudement sa lecture.
 
# La métaphore  de l'usine   

La production logicielle est en de nombreux points similaire à une production 
industrielle, où chaque membre de l'équipe et chaque process peut s'apparenter à une machine, 
à un capteur, le produit final étant bien sûr un logiciel livré à l'utilisateur. 
Cette métaphore combine deux grands aspects de l'industrie, la 
production de produits manufacturés et la [production par projet](https://en.wikipedia.org/wiki/Project_manufacturing).    

     
### La genèse 

Côté industriel, la commande a pu être passée
 avant qu'un besoin particulier n'ait été formulé par un client, sur la base 
 de prévisions de ventes. On parle  alors de **flux poussé**. 
 Une fois le produit fabriqué, nul ne dit qu'on
 trouvera client, et le produit risque d'engendrer des frais de stockage,
 voire de devenir obsolète ou se détériorer. 
 À l'opposé, le processus de fabrication peut être déclenché lors de la 
 commande. On parle alors de **flux tiré**. Il est indéniable que ce dernier 
 a de gros avantages [^1], et nous nous concentrerons sur ce processus ici. 
 
 
Côté logiciel, un besoin logiciel est exprimé par une entité. Cette entité 
 peut être  un utilisateur du logiciel, un représentant de la maîtrise d'
  ouvrage, voire par un développeur. 
      
La métaphore touche déjà juste, si personne n'a demandé ce produit, ou s'il 
a été produit trop lentement, vous risquez de ne passer à côté du besoin 
 utilisateur. De plus chaque 
  
  
### La production
   
  Côté industriel, il est nécessaire de rapprocher géographiquement les machines pour les  


Dans cette métaphore, le cahier des charges, le document word à l'ancienne de 800 pages est un ensemble
de matériaux de base.  Après 6 mois à être produit, il serait poussé ensuite devant 
un développeur pour qu'il commence à le transformer en un logiciel.


Au sens Lean, ce cahier des charges constitue donc un stock, donc une perte d'argent.
 
Dans une gestion de projet traditionnelle, si le produit est à 25% réalisé, 
il est rarissime qu'un utilisateur ait déjà utilisé le logiciel en cours de développement. 
Dans un projet agile, 25% des fonctionnalités du scope final sont implémentées, 
en production, et ce sont évidemment les fonctionnalités les plus prioritaires.    

 
 
 
 
 [^1] il faut néanmoins veiller à avoir un [changeover](https://en.wikipedia.org/wiki/Changeover) 
      extrêmement rapide et un stock de matières premières suffisant pour 
      répondre à un demande accrue.