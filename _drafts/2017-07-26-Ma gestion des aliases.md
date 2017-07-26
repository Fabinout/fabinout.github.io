---
layout: post
title: "Ma gestion des aliases"
description: "Guide, comment je gère mes alias dans le terminal"
category: 
tags: [Tools]
---

Je me retrouve souvent à changer de mission, et à changer d'environnement de travail.    
Voici comment j'ordonne mes **alias** dans mon terminal.


####~/.profile
```Bash
if [ -f ~/.bash_aliases ]; then
    . ~/.bash_aliases
fi
```

Le fichier .profile, chargé au lancement du terminal vérifie la présence d'un fichier **~/.bash_aliases**, et le source.

####~/.bash_aliases
```Bash

#Meta
alias aliases='cat ~/.bash_aliases'
alias ua='source ~/.bash_aliases'
``` 

Je rajoute ce fichier dans mes fichiers Favoris sur IntelliJ (add to Favorites (⌥⇧F)), 
et j'y accède via l'écran
des fichiers favoris (⌘2).

###Quand est-ce que je rajoute des alias dans mon fichier ?

Tout le temps.    
J'ai toujours d'ouvert dans un éditeur de texte simple (ou un scratch file dans IntelliJ (⇧⌘N)).    
Lorsque je tape quelque chose dans le terminal, je le colle d'abord dans mon fichier temporaire. Si la ligne que je colle 
s'y trouve déjà, c'est que c'est une commande que je risque de réutiliser. Il faut donc la rajouter à mes alias.

###Comment je choisis mes raccourcis ?
* Les raccourcis doivent être courts.    
* Tous mes alias similaires commencent par la même lettre, les raccourcis maven par 'm' par exemple, ceux de git commencent par 'g'.
* Comme il faut appuyer ensuite sur la touche entrée avec l'auriculaire droit, j'essaie de trouver un raccourci qui:
    - a du sens
    - finit par une lettre que je peux taper avec la main gauche
   
