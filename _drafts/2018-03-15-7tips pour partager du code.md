---
layout: post
title: "7 tips pour partager du code à l'écran"
description: "Un guide pour ceux qui font des katas de live-programming, du mob-programming en équipe ou simplement une démo?"
tags: [Tools, Démo, Kata, mob-programming]
---
    
Tout développeur se retrouvera un jour à montrer du code. Ça peut être au moment de faire une démo de la
dernière technologie à la mode sur laquelle vous avez passé votre week-end pluvieux.
Ça peut être lors d'un Kata de TDD que vous souhaitez montrer à vos collègues, où ça peut être votre premier talk
à Devoxx France.

Lors de cette occasion il est important de toujours garder à l'esprit le confort de lecture de vos spectateurs.

L'affichage de code comprend **aussi les commandes dans le terminal**. Il est courant
dans les conférences qui comportent du live-coding d'afficher son terminal pour faire
une démonstration, et il ne faut pas négliger la lisibilité de votre démo.

## Le confort de lecture avant tout

Gardez en mémoire que les conditions de visionnage de code ne sont pas les mêmes lorsque
l'utilisateur est à 30 centimètres de son écran que lorsqu'il est au fond de la salle et qu'il regarde le code projeté sur un écran
plat à 5 mètres de lui.

#### 1. Utilisez un fond clair

La majorité du contenu disponible sur Internet (wikipedia, blogs, docs,...)
est présenté avec du texte noir sur un fond clair. Or,
[la majorité](https://insights.stackoverflow.com/survey/2015) des développeurs utilise
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
et il est plus facile de lire un texte sur un fond clair.

C'est une manière facile d'adapter le style à votre contenu.

#### 2. Augmentez la taille de la police

Et augmentez-la encore. Il semble que la bonne taille soit d'à peu près **20 lignes** à
l'écran. Ça peut vous sembler énorme, mais gardez une pensée pour les
gens au fond de la salle.

Observez par exemple la présentation de DDD par Thomas Pierrain et Bruno
Boucard à Bdx.io 2017.

![livecoding par Boucard et Pierrain](/images/ddd pierrain.jpg "Un exemple de livecoding")

La caméra se trouve ici au pied de l'estrade, vous imaginez que quelqu'un se trouvant
au 10ème rang aura bien du mal à lire l'écran.

Ma règle générale que je m'inflige :

> Le contenu textuel reste lisible quand je
me tiens à 2 mètres de mon écran.

Évidemment, la ligne ne doit pas dépasser de l'écran en largeur.
Si vous utilisez une IDE, je vous suggère d'utiliser simplement le "Mode Présentation".

#### 3. Utilisez une coloration syntaxique simple, ou n'en utilisez pas

Une coloration syntaxique permet aux participants de reconnaitre d'un coup d'œil
les éléments importants de la syntaxe du langage que vous utilisez. 

**Il vaut mieux ne pas avoir de coloration syntaxique qu'une mauvaise coloration
syntaxique.**

*Instant vis-ma-vie de daltonien* : j'avais personnalisé la coloration syntaxique
de mon IDE, et j'avais mis sans le savoir les erreurs de compilation en "souligné-vert".

*Résultat* : les collègues qui codaient sur mon clavier durant un dojo mettaient du
temps à réaliser qu'ils avaient écrit un code qui ne compilait pas.

![Exemple de mauvaise coloration syntaxique](/images/coloration syntaxique.png "Un exemple de mauvaise coloration syntaxique")

Plusieurs choses à dire ici :

le rouge foncé est illisible



#### 4. Maximiser la facilité à pointer une partie de votre code

Un problème récurrent dans le cas d'un live-coding c'est la capacité à retrouver le
curseur du présentateur, surtout dans le cas où beaucoup de refactoring 










https://ux.stackexchange.com/a/53268
http://uxmovement.com/content/when-to-use-white-text-on-a-dark-background/


