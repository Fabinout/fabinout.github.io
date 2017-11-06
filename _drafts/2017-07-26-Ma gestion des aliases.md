---
layout: post
title: "Ma gestion des aliases"
description: "Ccomment je gère mes alias dans le terminal"
category: 
tags: [Tools]
---

Je me retrouve souvent à changer de mission, et à changer d'environnement de travail.    
Je vais vous présenter comment j'ordonne mes **alias** dans mon terminal Mac.    
Tout d'abord, qu' est-ce qu'un alias ?

##### Définition d'un alias selon https://ubuntu-fr.org

> Un alias est une substitution abrégée de commandes répétitives et/ou longues à taper dans la console. 

Au travail!

### Le matériel

Je commence par créer deux fichiers, le premier, le **.profile** contiendra principalement des méthodes utilitaires
 (auto-complétions, paramètrage des couleurs, ...), des alias et des variables d'instance. 
 Une des méthodes qui m'intéresse particuliètement nous permet de*sourcer*un autre fichier, c'est à dire
 de copier le contenu du fichier spécifié en argument à l'endroit où la commande est invoquée.    
 Pour les nuls, ça signifie qu'on peut découper ses fichiers de profile comme on le souhaite. 

##### ~/.profile
```Bash
if [ -f ~/.bash_aliases ]; then
    source ~/.bash_aliases
fi
```
> Tip : ```source``` et ```.``` sont des synonymes en bash, mais source est plus visible, donc plus lisible.


Le fichier .profile, chargé au lancement du terminal vérifie la présence d'un fichier **~/.bash_aliases**, et le source
 s'il est présent. On peut donc centraliser tous nos aliases dans un fichier externe. Libre à nous ensuite de ségréguer
  à nouveau les 
 raccourcis de ce fichier selon les technos utilisées.
  
  Enfin, je créer un fichier aliases et j'y rajoute systématiquement les deux alias suivants. 

##### ~/.bash_aliases
```Bash

#Meta
alias la='cat ~/.bash_aliases'
alias ua='source ~/.bash_aliases'
``` 
La commande ```la``` permet de de lister les alias sauvegardés, la commande ```ua``` permet de raffraichir ses alias 
sans redémarrer son terminal. 


> Tip, il existe la commande ```alias``` permettant de lister tous vos aliases. Quand la liste  devient conséquente, 
il est plus facile de séparer les alias selon les domaines ou technos, et d'avoir un raccourci pour afficher un seul 
type d'alias.    
Par exemple ```alias lb='cat ~/.bash_aliases_mongodb & cat ~/.bash_aliases_mysql``` 

### La méthode

Je rajoute ces fichier dans mes fichiers Favoris sur IntelliJ (add to Favorites (⌥⇧F)), 
et j'y accède via l'écran des fichiers favoris (⌘2). Selon les cas, je peux aussi avoir un alias me permettant d'ouvrir
le fichier des alias dans IntelliJ pour l'y éditer directement: ```alias ia='idea ~/.bash_profile'```. 


##### Quand est-ce que je rajoute des alias dans mon fichier ?

Tout le temps.    

Attention, je n'ai pas dit "très souvent", j'ai bien dit tout le temps. 

J'ai toujours d'ouvert dans un éditeur de texte simple (ou un scratch file dans IntelliJ (⇧⌘N)).    
Lorsque je tape une quelconque commande dans le terminal, je le colle d'abord dans 
mon fichier temporaire. Si la ligne que je colle y est déjà présente à l'identique, c'est que c'est une commande que 
je risque de réutiliser. Il faut donc la rajouter à mes alias.

##### Comment je choisis mes raccourcis ?
* Les raccourcis doivent être courts.    
* Tous mes alias similaires commencent par la même lettre, les raccourcis maven par 'm' par exemple, ceux de git commencent par 'g'.
* Comme il faut appuyer ensuite sur la touche entrée avec l'auriculaire droit, j'essaie de trouver un raccourci qui:
    - a du sens
    - finit par une lettre que je peux taper avec la main gauche (pour ensuite taper sur la touche entrée)
    
       
