---
layout: post
title: "Un logiciel qui marche"
description: "Working software over comprehensive documentation"
category: 
tags: [Clean Code, Agilité]
---

Parlons un peu d'un des 4 piliers de l'agilité. 

> **Working software** over comprehensive documentation    

Pour clarifier tout de suite, ce pilier de l'agile **ne dit pas** qu'il ne faut pas rédiger 
de documentation. L'objectif de l'agile est de fournir de la meilleure manière possible 
un logiciel à des utilisateurs, et d'être capable de modifier son process régulièrement. 
Cet adage vise donc à reconcentrer les efforts des membres de l'équipe 
autour du produit final, **un logiciel qui marche**.    

Cet article se base sur ma lecture récente de **Le but : Un processus 
de progrès permanent** de Eliyahu Goldratt : [Lien amazon](https://www.amazon.fr/but-processus-progr%C3%A8s-permanent/dp/2124654047).   
Je vous le conseille chaudement sa lecture, ne serait-ce que pour prendre du recul sur la mode du lean IT.
 
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
 possède des avantages évidents, et nous nous concentrerons sur ce processus ici. 
 
 
Côté logiciel, un besoin logiciel est exprimé par une entité. Cette entité 
 peut être  un utilisateur du logiciel, un représentant de la maîtrise d'
  ouvrage, voire un développeur. 
      
Si personne n’a commandé ce produit, ou s’il a été produit trop lentement, 
vous risquez de passer à côté du besoin utilisateur, 
donc de produire un logiciel déjà présent chez la concurrence, ou pire inadapté à son besoin. 
  
  
### La production
   
  
Si l'on devait comparer la production de code informatique à une industrie, alors 
**le cahier des charges serait l'ensemble
des matériaux de base**.  Après un certain temps à être produit, il serait poussé ensuite devant 
un développeur pour qu'il commence à le transformer en un logiciel.

Au sens Lean, ce cahier des charges constitue donc un stock, et donc une perte d'argent.
 
Dans une gestion de projet traditionnelle, si le produit est à 25% réalisé, 
il est rarissime qu'un utilisateur ait déjà utilisé le logiciel en cours de développement. 
Dans un projet agile, 25% des fonctionnalités du scope final sont implémentées et sont utilisables 
en production, elles constituent les fonctionnalités les plus prioritaires.    
 
   
### Le flux tiré

Il a été très vite théorisé l'intérêt du **flux tiré** (ou "juste-à-temps", "just-in-time", ou "jit") 
 dans l'industrie automobile des années 50. Cette méthode d'organisation de la production industrielle 
  vise à minimiser les stocks et les en-cours de fabrication entre l'arrivée de la matière première à la livraison 
  des produits finis. Cette méthode s'appelle aussi la méthode des 5 zéros (_zéro panne, zéro délai, zéro papier, zéro stock, zéro défaut_).
  
 
 Après un certain temps d'adaptation, 
 les avantages ont été perçus : 
 * Une organisation adaptée à l'évolution constante des besoins des clients
 *  Peu ou pas de constitution de stocks, qui on le sait sont couteux en trésorerie et 
 portent le risque de n'être jamais utilisés ou vendus
 

Il est facile de voir que dans notre industrie informatique, l'implémentation de ces méthodes d'organisation modernes 
pourrait nous aider à résoudre les problèmes récurrents de temps de livraison, de temps de recette et de qualité logicielle. 
Si on prêtait plus attention à la livraison d'un logiciel utilisable, ainsi qu'à la mise en place
de bonnes pratiques, la livraison zéro-défaut pourrait devenir quotidienne. 




 Merci [Arnaud Bailly](https://github.com/abailly) pour avoir inspiré la rédaction de cet article
