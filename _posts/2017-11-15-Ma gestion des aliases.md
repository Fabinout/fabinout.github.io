---
layout: post
title: "Ma gestion des alias"
description: "Comment je gère mes alias dans le terminal"
tags: [Tools, Terminal]
---

Je me retrouve souvent à changer de mission, et à changer d'environnement de travail.    
Je vais vous présenter comment j'ordonne mes **alias** dans mon terminal Mac.    

## Introduction : pourquoi utiliser des alias ?

Ceux et celles qui se rappellent de leurs premiers pas dans une console ou un terminal le savent, la navigation y est complexe, 
les boutons inexistants, et la souris inutile. Les néophytes face à cet outil cryptique et effrayant, où les coquilles 
sont impitoyables, se trouveront donc souvent perplexes devant cette popularité chez leurs collègues plus expérimenté·e·s.      
C'est qu'il est bien plus facile de se déplacer dans une arborescence de fichier avec la souris qu'avec des 
lignes de commande.     
Néanmoins, avec un peu de pratique il devient très aisé de manipuler sa machine via la console. Malheureusement, il subsiste
quelques douleurs :    
* les fautes de frappes sont punitives (même si l'auto-complétion peut aider) ;
* les commandes sont très nombreuses, ne sont pas facilement mémorisable, et ont plusieurs options et flags optionnels à apprendre ;
* les commandes saisies au long de la journée sont répétitives.   
 
 
Pour résoudre ce problème vous pouvez créer des alias sur votre machine.


### Définition d'un alias selon https://ubuntu-fr.org

> Un alias est une substitution abrégée de commandes répétitives et/ou longues à taper dans la console. 


Au travail!

## Les fichiers à créer

Je commence par créer deux fichiers, le premier, le **.profile** contiendra principalement des méthodes utilitaires
(auto-complétions, paramètrage des couleurs, ...), des alias et des variables d'instance. 
Une des méthodes qui m'intéresse particuliètement nous permet de *sourcer* un autre fichier, c'est à dire
de copier le contenu du fichier spécifié en argument à l'endroit où la commande est invoquée.    
Pour les nuls, ça signifie qu'on peut découper ses fichiers de profile comme on le souhaite. 



### ~/.profile

<script src="https://gist.github.com/Fabinout/58f3326b4d01d02352e4b184a47abc43.js"></script>
 
> Tip : ```source``` et ```.``` sont des synonymes en bash, mais source est plus visible, donc plus lisible.



Le fichier .profile, chargé au lancement du terminal vérifie la présence d'un fichier **~/.bash_aliases**, et le source
s'il est présent. On peut donc centraliser tous nos aliases dans un fichier externe. Libre à nous ensuite de ségréguer
à nouveau les raccourcis de ce fichier selon les technos utilisées.
  
Puis, je crée un fichier contenant les aliases et j'y rajoute systématiquement les deux alias suivants. 

### ~/.bash_aliases

<script src="https://gist.github.com/Fabinout/df651d9a0734eca3eb04cf1e47310e13.js"></script>
 
La commande ```la``` permettra de lister les alias sauvegardés, et ```ua``` permet de raffraichir ses alias 
sans redémarrer son terminal.   

N'oubliez pas de sauvegarder ces documents sur un repository, ils constituent une part importante de la capitalisation
de votre expérience dans le terminal.

### La commande 'alias'
 
Il existe la commande ```alias``` permettant de lister (vous l'avez deviné) tous vos aliases. 
Les inconvénients étant que :  
* quand la liste  devient conséquente, la liste de tous les alias peut ne pas être pratique à parcourir ;
* les éventuelles commentaires (commençant par ```#```) ne sont pas affichés ;    
* une utilisation efficace nécessite de faire ```alias | grep mvn``` ce qui n'est pas pratique à taper rapidement.    
  
Il est plus facile de séparer les alias selon les domaines ou technos, et d'avoir un raccourci pour afficher un seul 
type d'alias.    
Par exemple ```alias lb='cat ~/.bash_aliases_mongodb & cat ~/.bash_aliases_mysql```   

## La méthode

Cette partie peut sembler superflue, mais c'est là que réside tout l'intérêt de ma méthode de gestion des alias.      
La création de fichiers d'alias et l'organisation dans des sous-fichiers est tout au plus pratique, mais ne me sert 
strictement à rien si je ne dump pas mes commandes régulièrement dans ces fichiers. La suite de cet article sera donc 
consacrée à l'organisation de la persistence de mes alias.
       
Je rajoute ces fichier dans mes fichiers Favoris sur IntelliJ (add to Favorites (⌥⇧F)), 
et j'y accède via l'écran des fichiers favoris (⌘2).          
Dans les rares cas où je n'ai pas lancé IntelliJ, j'ai aussi un alias me permettant d'ouvrir
le fichier des alias dans IntelliJ pour l'y éditer directement: ```alias ia='idea ~/.bash_profile'```. 


### Quand est-ce que je rajoute des alias dans mon fichier ?

Tout le temps.    
Attention, je n'ai pas dit "très souvent", j'ai bien dit tout le temps. C'est beaucoup plus dur qu'il n'y parait de se 
débarasser de ses mauvaises habitudes, c'est aussi un des plus gros freins d'adoptions de
[la méthode GTD](https://fr.wikipedia.org/wiki/Getting_Things_Done), que je vous 
suggère d'étudier.  

Je garde constamment ouvert un fichier qui compile les commandes tapées au clavier (y compris les commandes 
de déplacement dans les répertoires) dans mon terminal.    
Avant de taper une quelconque commande dans le terminal, je la colle d'abord dans mon fichier. 
Si la ligne que je colle y est déjà présente à l'identique, c'est que c'est une commande que 
je réutilise. Il faut donc la rajouter à mes alias.

#### Bonus : quel alias pour quelle commande ?

Ci-dessous les critères que j'utilise pour choisir les mots-clés qui constitueront mes alias :
* Les raccourcis doivent être courts ;    
* tous mes alias similaires commencent par la même lettre, les raccourcis maven par 'm' par exemple, ceux de git commencent par 'g' ;
* comme il faut appuyer ensuite sur la touche entrée avec l'auriculaire droit, j'essaie de trouver un raccourci qui :
    * a du sens car c'est évidemment important de se rappeler de ses alias (par exemple ```alias dpa='docker ps -a'```), 
    * finit par une lettre que je peux taper avec la main gauche.
    