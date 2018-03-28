---
layout: post
title: "12 tips pour partager du code à l'écran"
description: "Un guide pour ceux qui font des katas de live-programming, du mob-programming en équipe ou simplement une démo?"
tags: [Tools, Démo, Kata, mob-programming]
---
    
Tout développeur se retrouvera un jour à montrer du code. Ça peut être au moment de faire une démo de la
dernière technologie à la mode sur laquelle vous avez passé votre week-end pluvieux.
Ça peut être lors d'un Kata de TDD que vous souhaitez montrer à vos collègues, où ça peut être votre premier talk
à Devoxx France.

Lors de cette occasion il est important de toujours garder à l'esprit le confort de lecture de vos spectateurs.
Et ce confort dépend des conditions de visionnage de code qui ne sont pas les mêmes lorsque
l'utilisateur est à 30 centimètres de son écran, lorsqu'il est au fond de la salle de conférence, ou lorsqu'il regarde
le code projeté sur un écran plat dans une salle de réunion orientée sud.

L'affichage de code comprend **aussi les commandes dans le terminal**. J'observe souvent dans les conférences techs un
présentateur afficher son terminal, il est beaucoup plus rare que je comprenne
ce qui se passe à l'écran.

## Le confort de lecture avant tout

Gardez en mémoire que les conditions de visionnage de code ne sont pas les mêmes lorsque
l'utilisateur est à 30 centimètres de son écran que lorsqu'il est au fond de la salle et qu'il regarde le code projeté sur un écran
plat à 5 mètres de lui.

#### 1. Utilisez un fond clair

La majorité du contenu disponible sur Internet (wikipedia, blogs, docs,...)
est présenté avec du texte noir sur un fond clair. Or,
[la majorité](https://twitter.com/Fabinout/status/977151283445592064) des développeurs utilise
un fond sombre à la Darkula ou anthracite. D'où vient cette discordance ?

Le thème Dark est souvent apprécié des jeunes développeurs qui ont encore de bons yeux et passent
la journée face à leur écran. Dans un bureau qui n'est pas spécialement éclairé,
l'écran devient la source principale de luminosité, et le travail de longue durée face à un
écran clair fatigue les yeux. Dans cette situation, un fond sombre avec une police claire (mais
pas blanche pour limiter le contraste) est une situation très confortable pour les yeux.

Si cette configuration est plus reposante sur de longues durées et dans des conditions
particulières, elle est plus fatigante dans la majorité des situations.

> White stimulates all three types of color sensitive visual receptors in the human eye
in nearly equal amounts. It causes the eye to focus by tightening the iris.
Since the eye is focused, dark letter forms on light backgrounds are easier to read.
When using a dark background with strong light letter forms, the iris opens to allow
more light in, but that causes letter forms to blur.

![Un texte noir sur fond blanc, et un texte blanc sur fond noir](/images/light-absorb-reflect-text.png "Comparaison de paragraphes")

Un fond sombre est donc rarement adapté à des présentations de code
sur grand écran ou rétroprojecteur. Vos spectateurs ne seront pas nécessairement dans
l'axe de l'écran et seront éblouis par le moindre reflet sur un écran sombre. Si vous codez
de temps en temps depuis votre terrasse ensoleillée, vous savez qu'un fond sombre est
simplement inutilisable dans ces conditions là.

Pour information, l'œil humain a deux fonctions : il peut **lire** et **scanner**. Il va lire
un paragraphe, c'est à dire passer sur tous les mots pour comprendre le sens global, mais va
scanner un titre en le visualisant dans son ensemble.
Comme le dit cet article sur [UXMovement](http://uxmovement.com/content/when-to-use-white-text-on-a-dark-background/),
il est plus facile de scanner un texte court avec une police blanche sur fond coloré,
et il est plus facile de lire un texte sur un fond clair. Dans un slide de présentation, c'est une manière facile
 d'adapter le style à votre contenu.

#### 2. Augmentez la taille de la police

Et augmentez-la encore. Il semble que la bonne taille soit d'à peu près **20 lignes** à
l'écran. Ça peut vous sembler énorme, mais gardez une pensée pour les
gens au fond de la salle.

Observez par exemple la présentation de DDD par Thomas Pierrain et Bruno
Boucard à Bdx.io 2017.

![livecoding par Boucard et Pierrain](/images/ddd pierrain.jpg "Un exemple de livecoding")

La caméra se trouve ici au pied de l'estrade, vous imaginez que quelqu'un se trouvant
au 10ème rang aura bien du mal à lire l'écran.

La règle générale que je m'inflige :

> Le contenu textuel reste lisible quand je
me tiens à 2 mètres de mon écran de laptop.

Évidemment, la ligne ne doit pas dépasser de l'écran en largeur.
Si vous utilisez un IDE, je vous suggère d'utiliser simplement le "Mode Présentation" pour gagner de la place
en cachant les différentes barres et menus.

#### 3. Utilisez une coloration syntaxique simple, ou n'en utilisez pas

Une coloration syntaxique permet aux participants de reconnaitre d'un coup d'œil
les éléments importants de la syntaxe du langage que vous utilisez. Néanmoins, la couleur
de ce que vous montrez a généralement peu d'importance, il est plus important que le
contenu textuel soit lisible par tous.

**Il vaut mieux ne pas avoir de coloration syntaxique qu'une mauvaise coloration
syntaxique.**

*Anecdote vis-ma-vie de daltonien* : j'avais personnalisé la coloration syntaxique
de mon IDE et avais mis sans le savoir les erreurs de compilation en souligné-vert.

*Résultat* : les collègues qui codaient sur mon ordinateur durant un coding-dojo
mettaient du temps à réaliser qu'ils avaient écrit un code qui ne compilait pas.

Voici un exemple à ne pas suivre :

![Exemple de mauvaise coloration syntaxique](/images/coloration syntaxique.png "Un exemple de mauvaise coloration syntaxique")

Entre autres :

* le rouge foncé sur fond noir est illisible
* l'orange clair sur fond blanc est illisible
* le bleu sur fond noir est difficile à lire pour un daltonien


## Le confort de navigation dans votre code

Dans le cas d'un live-coding, il est courant de peiner à retrouver le
curseur du présentateur, surtout dans le cas où beaucoup de refactoring
se passent à l'écran dans un court laps de temps.
Pour aider le spectateur à vous situer dans le code affichée, voici plusieurs astuces :

#### 4. Affichez les numéros de lignes

Avec les numéros de lignes, vous pourrez facilement décrire ce que vous êtes en train de faire pour
aider vos spectateurs à se revenir dans la présentation même s'ils se sont décrochés.

![code de gilded rose inn](/images/linenumber.jpg "des numéros de ligne")

*La condition de la ligne 49 fait doublon avec la condition de la ligne 39, vous voyez ?*

#### 5. Surlignez la ligne courante

Il est possible dans les applications JetBrains de surligner la ligne
sur laquelle est votre curseur, pour ainsi retrouver en un coup d'œil ce
que le présentateur est en train de modifier. Il est aussi possible de l'
encadrer comme l'ont fait Bruno Boucard et Thomas Pierrain plus haut.

![code de gilded rose inn](/images/surligne.jpg "une ligne surlignée")

Cette option se trouve dans les propriétés de coloration de l'éditeur :
![préférences intellij](/images/caret row.jpg "settings de la couleur caret row")

#### 6. Utilisez un curseur bloc plutôt qu'un curseur l

![un bloc caret](/images/caret.jpg "un bloc caret")

En utilisant un block caret avec un clignotement lent, vous pouvez encore donner un dernier coup de
pouce au spectateur assoupi à retrouver le fil de votre refactoring.
Vous pouvez modifier ce paramètre dans les paramètres de l'éditeur.

![caret settings](/images/useblockcaret.jpg "paramètres du curseur")

#### 7. Autorisez le placement en fin de ligne

Cette option permet comme son nom l'indique de laisser le curseur se placer
indistinctement après la fin d'une ligne de code.

![end of line caret](/images/2018-03-26 23_44_30.gif "curseur après la fin de la ligne")

Mon avis sur cette option est mitigé. D'une part elle permet de rendre le
déplacement vertical au sein du code source plus fluide. D'autre part,
c'est une option qui est déstabilisante en coding-dojo car les participants
ont l'habitude d'aller vers la droite en fin de ligne pour passer à la
ligne suivante.  Ça signifie aussi que vous aussi, présentateur, devrez
réapprendre à naviguer dans votre code avec cette option.

![caret setting](/images/caretsetting.jpg "parametre du curseur en fin de ligne")

## Une présentation de code... est une présentation quand même

Vous avez surement fait une présentation ou une soutenance durant vos études et votre carrière. Dans ces
cas là, comme dans le cas d'une présentation de code à une conférence il y a la règle des trois P.

* la préparation    
* la préparation
* la préparation

#### 8. Planifiez votre démonstration 

Listez les étapes importantes de votre démo, et gardez la liste accessible à portée de main. Ainsi vous pourrez y revenir
au moindre doute.

#### 9. Versionnez votre code

Vous êtes un développeur, la probabilité est élevée que vous sachiez maitriser **git** alors profitez-en. Versionnez
votre code, et vérifiez que vous pouvez à tout moment revenir à un état **qui marche.**   De nombreux guides (par exemple [Code Demo using git](http://programmaticallyspeaking.com/code-demo-using-git.html)) 
existent pour vous expliquer comment vous y prendre. Vous pouvez adopter l'outil à votre utilisation en 
utilisant librement des alias ou des tags.

#### 10. Si vous ne pouvez pas garder un code dans un état fonctionnel, vous avez d'autres options

Si vous faites une application Android/Unity qui fait de la
réalité augmentée en scrappant les données de votre API custom, votre démo peut planter pour des dizaines de façons différentes 
(internet ne marche pas, votre téléphone n'a pas de batterie, etc.).
Dans ces situations où un versionning de votre code applicatif ne permet pas de couvrir toutes les situations, il ne vous
reste qu'à garder sur votre poste une vidéo de votre démo fonctionnelle, mais c'est toujours mieux que de regarder ses pieds
en disant que "là normalement ça aurait du marcher".

#### 11. Evitez les distractions

On a tous déjà vu un présentateur recevoir un tweet durant une présentation, un email ou encore un message Slack rigolo.
Dans le meilleur des cas le message est banal, peu intéressant.
Dans la majorité des cas, vous allez inconsciemment lire la notification, et interrompre votre flux de pensée. Selon
votre aisance, vous pouvez continuez votre phrase comme si de rien n'était, ou bien perdre le fil de votre phrase et commencer
à bégayer.
Dans certains rares cas (mais déjà arrivés), vous pouvez recevoir un message salace de votre conquète du week-end précédent.

Il y a peu de chance que vous ayez besoin de Twitter ou Facebook durant votre présentation, évitez-vous des galères et
fermez vos onglets et applications de réseaux sociaux avant de commencer votre présentation.

#### 12. Travaillez votre rythme

Selon le thème de votre présentation de code, vous pouvez accélérer ou décélérer à votre convenance, libre à vous de faire
plusieurs Ctrl+Z et de refaire vos manipulations si vous sentez que vous êtes allé un peu vite et que vous avez perdu votre
public. Certains moments sont propices à l'utilisation d'un template ou d'un copier-coller, d'autres non.  
Discerner les étapes clés de votre présentation pour accélérer celles qui ont peu de valeur-ajouté ou au contraire appuyer ceux qui sont
critiques à votre présentation.

