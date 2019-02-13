---
layout: post
title: "Les lois de l'informatique"
description: "Trouve la réponse à toutes les questions de ton client"
category:
tags: [Consulting, satire]
---

Si tu es consultant débutant, l'important est d'identifier, puis de résoudre les problèmes de ton client.
Si tu as de l'expérience (et du cynisme), l'important c'est d'avoir réponse à tout. Plus la réponse est péremptoire,
mieux c'est. Pas besoin d'empathie, pas besoin de réflexion, si on a dans sa poche la loi si possible obscure qui identifie
son problème. Tu seras tenté de proposer une solution, mais retiens-toi. L'important c'est de montrer son
savoir de consultant, surtout pas de s'exposer en tentant de corriger le problème.
Et surtout, ça te permet d'étaler l'étendue de ton savoir infini.

Ami consultant, ne cherche pas plus loin, voici la liste des choses à savoir pour pouvoir briller dans la société de ton
client, et l'asperger de ta connaissance à la moindre occasion.

# Les lois connues

Attention, à n'utiliser qu'avec parcimonie car le client les connaît probablement. Ça ne te permettra donc pas de
justifier ton TJM de consultant.

## Loi de Murphy

>Tout ce qui peut aller mal, se passera mal.

On ne la présente plus, cette loi était déjà présente dans les chaines de mail qu'on se transférait dans
les années 90, à la grande époque des blagues sur Chuck Norris et des demotivational posters. En fait j'en
sais rien parce que j'étais pas né, mais c'est ce que me racontait ma grand-mère.

À utiliser lorsque tu observes que rien ne va chez le client et qu'il est dans une situation catastrophique à cause
de ses choix tous plus idiots les uns que les autres.

## Loi de Moore

> Quelque chose double tous les dix-huit mois

L'intérêt de cette loi vient de son extrême versatilité. Il faut juste trouver quelque chose qui double de temps en temps
et s'en servir pour tirer une loi générale.

* Le nombre d'employé double tous les ans dans les startups
* La puissance des semi-conducteurs double tous les ans
* Le nombre de transistors d'un microprocesseur double tous les 2 ans
* Le nombre de microservices de ton client double tous les 15 mois
* etc.

Même si ça double pas et que ça croit linéairement, ce n'est pas grave.

#### Corollaire de la loi de Moore

> Tout indicateur croissant peut suivre vaguement une loi de Moore


## Loi de Conway

> Les organisations qui définissent des systèmes ... sont contraintes de les produire sous des designs qui sont
des copies de la structure de communication de leur organisation

À noter que l'architecture logicielle est une structure de communication, autrement dit la façon
de travailler de l'entreprise à une influence directe sur l'organisation de votre SI. Melvin Conway a exprimé
cette loi en 1967, quand le système d'information représentait quelque chose fondamentalement différent d'un SI en 2019.
Mais un bon consultant ne s'inquiète pas de ces problèmes d'anachronisme, si tu observes que les
différentes équipes du client n'arrivent pas à collaborer, alors tu peux aisément dégainer ta Loi
de Conway toute neuve.

## Syndrome de l'imposteur

> Les personnes atteintes du syndrome de l'imposteur, appelé aussi syndrome de l'autodidacte, expriment une forme de
doute maladif qui consiste essentiellement à nier la propriété de tout accomplissement personnel.

En substance, un individu atteint de ce syndrome attribuera ses qualités ou succès au favoritisme de ses chefs,
à la chance ou encore à la discrimination positive. Ne laisse pas le doute s'installer.
Comment t'en servir au
quotidien ? Deux manières :
* Quand ton client te dit qu'il ne comprend pas certaines problématiques, rassure-le en lui disant qu'il n'est
pas bête et que c'est sûrement un syndrome de l'imposteur, évidemment que ce problème simple de développement logiciel est à sa
portée. Après tout si un développeur le comprend, pourquoi pas lui !
* Tu n'as pas bossé ta restitution client ? Tu cherches tes mots et tu n'arrives pas à convaincre ? C'est la faute
de ton syndrome de l'imposteur. Ça ne peut pas être la faute d'un manque de travail, encore moins d'un manque de
connaissance.


# Les lois que tu connais mais que tu ne connais pas le nom

Ces lois sont instinctives, elles décrivent des truismes comme les autres, mais ont l'avantage de faire pompeux.
Moins pompeux qu'utiliser le mot truisme, mais quand même.

## Loi de Goodhart

> Lorsqu'un indicateur devient une cible, il cesse d'être une bonne mesure.

Si tu utilise une mesure comme un objectif à atteindre, alors elle influence vos décisions, car le but n'est plus
d'améliorer la qualité du travail fourni, le but devient d'atteindre l'indicateur.

### Corollaire : loi de Campbell

> plus un indicateur quantitatif est utilisé pour la prise de décision, plus il a de chances de fausser et
corrompre le processus qu’il a pour objet de surveiller


Si tu choisis un indicateur comme objectif, alors tu atteindras cet objectif. La production globale
ou le rendement global ne sera pas améliorée, mais l'effort sera portée spécifiquement sur le KPI
(abuse des anglicismes, tu es consultant, pas académicien) sans prendre en compte l'*esprit* du KPI.

Quelques exemples  :

* Si tu mesures la qualité logicielle en nombre de bug, tu n'auras plus de bug, mais tu auras des "demandes d'évolutions"
* Si tu mesures la qualité logicielle en statistique sonar, alors les équipes passeront leur mois de décembre à nettoyer le code
pourri qu'elles auront codé tout au long de l'année
* Si tu mesures la qualité logicielle en pourcentage de couverture de code, alors tes équipes feront des tests sans assertions
* Si ton objectif est de diminuer la latence de l'application, alors mets des caches partout. Peu importe
que les données datent d'hier.

*Pas besoin de comprendre la différence entre les deux lois, c'est un détail d'implémentation qui ne concerne
que le client.*

## Loi de Hoffstadter

> Quoi qu'il arrive tu seras en retard.

Rien de mieux que du cynisme et du défaitisme, peu importent la tache, le délai et la météo, quoi qu'il arrive : tu
seras en retard.

## Loi de Hoffstadter qui prend en compte la loi de Hoffstadter

> Quoi qu'il arrive tu seras en retard. Même si tu prends en compte la loi de Hoffstadter.

Même en prenant large pour les délais et en réduisant le scope, tu seras en retard. Sers toi de ce fatalisme
quand tu es en retard sur ton boulot.

## Principe de Peter

> dans une hiérarchie, tout employé a tendance à s'élever à son niveau d'incompétence

En partant du postulat qu'un employé compétent est promu (ce qui reste encore à prouver), tout employé compétent
recevra des promotions jusqu'à arriver à un poste qui exige des compétences qu'il n'a pas.
Comment peux-tu juger que quelqu'un est incompétent à son poste ? Rien à faire, c'est une phrase réflexe qui
est à sortir quand votre interlocuteur se plaint des compétences de ses collaborateurs.

> "Mon directeur de service sert vraiment à que dalle"
> "Ahah ouais, on est en plein dans le syndrome de Peter !"

## Principe de Dilbert

> Les gens les moins compétents sont systématiquement affectés aux postes où ils risquent de causer
le moins de dégâts : ceux de managers.

Les managers sont la cible idéale, ils ne produisent rien et ne peuvent donc rien casser.
Ce principe est une version aggravée du principe de Peter, et s'applique spécifiquement à l'incompétence des
managers. Une bonne blague entre ingénieurs.

## Effet Dunning-Krueger

> L’effet Dunning-Kruger, ou effet de surconfiance, est un biais cognitif selon lequel les moins qualifiés dans un
domaine surestiment leur compétence.

Ce biais a été popularisé par Coluche, citant Descartes, dans les années 1980 : « […] l'intelligence,
c'est la chose la mieux répartie chez les hommes, n'est-ce pas, parce que, quoiqu'il en soit
pourvu, il a toujours l'impression d'en avoir assez, vu que c'est avec ça qu'il juge, hein ! ». Coluche en 2019
est le nouveau Deleuze.

Contre toute attente ce biais est facilement trouvable chez les consultants qui balancent de grosses vérités
bien péremptoires à tout bout de champs, car il est plus efficace de dire quelque chose avec autorité que de nuancer
son propos.

* Si en 2019 t'as pas Kubernetes dans ton SI, alors t'as raté ta vie
* L'avenir c'est le cloud, l'on-premise c'est pour les banques et les loosers
* Si tu fais pas d'agile à l'échelle, tu sauras pas réagir assez vite au changement, t'es déjà mort
* Le HTTPS c'est facile, si tout ton SI est pas en HTTPS, c'est que tu fais pas d'effort

A l'inverse, l'effet Dunning-Kruger nous dit qu'une personne très compétente et intelligente sous-estimera
ses compétences, tout simplement parce qu'il a conscience de ses lacunes. Exemple : je connais très bien Java, mais
je n'ai pas l'habitude de fine-tuner le garbage-collector, donc j'estime être dans le top 25% des développeurs
Java.

## Loi de Parkinson

> Tout travail au sein de l'administration augmente jusqu’à occuper entièrement le temps qui lui est affecté

Cette loi s'applique initialement aux administration mais son usage s'étend au privé, particulièrement aux
réunions, si tu juges qu'on peut discuter d'un problème en 1H, alors il est physiquement impossible que
l'on sorte de cette réunion avant la fin.

## Loi de la trivialité de Parkinson

> Members of an organization give disproportionate weight to trivial issues

Aussi appelé "syndrome du garage à vélo", les managers étant incompétents par défaut, ils vont fournir un gros
effort pour influencer ou modifier l'élément le plus trivial qu'ils peuvent comprendre.

Dans le cas du garage à vélo, un comité doit travailler sur le budget pour la construction d'une centrale nucléaire,
le choix du modèle de réacteur nucléaire (qui concerne l'immense majorité du prix de la centrale en elle-même)
est traité très rapidement. Mais lorsqu'il faut discuter du garage à vélo pour les employés, tout le monde y va
de son avis sur la question "je pense qu'il faut peindre le garage en bleu", "on doit pas faire l'erreur de mettre un toit
sur le garage à vélo, ça sert à rien et ça fera fournaise en été", etc. Résultat la discussion dérisoire
accapare l'attention de 20 personnes pendant des heures.

Si un client s'attarde sur un détail où vous ne trouvez pas de réponse, ça permet de remettre en doute ses compétences
tout en évitant de répondre à la question. Une pierre deux coups.

## Systémantique de Gall

> A complex system that works is invariably found to have evolved from a simple system that worked. A complex system
designed from scratch never works and cannot be patched up to make it work. You have
to start over with a working simple system.

Si le why d'un projet est compliqué, alors le projet ne marchera pas. C'est une loi particulièrement efficace quand
on parle d'agile, l'objectif est de commencer par quelque chose d'utile et de simple, de l'utiliser et seulement
ensuite tenter de rajouter des fonctionnalités. Étant donné que tout est système, et que tout système est à l'intérieur
d'un autre système, on peut foutre des systèmes partout.

## Loi de Brook

> Ajouter des personnes à un projet en retard accroît son retard

Contrairement à la croyance populaire, on ne finit pas plus vite en rajoutant des *ressources* à l'équipe. La phrase
que vous devez dire ensuite est "1 femme fait un bébé en 9 mois, 9 femmes ne font pas 1 bébé en 1 mois"; ça a
rien à voir avec la gestion d'un projet informatique, mais ça fait golri à chaque fois.

## Culte du cargo

> Sommes-nous en train d'appliquer des méthodes par mimétisme d'autres entreprises, sans comprendre le bien-fondé de
ces actions ?

Le culte du cargo vient (selon la légende) de l'Océanie, plus précisément de la Mélanésie.
Dans ce pays, les aborigènes observent les bases militaires que fabriquent les militaires occidentaux et japonais, et
notent que peu après la construction de tour de contrôle et de radio, des avions survolent le secteur en parachutant
des caisses de vivre et d'armement. Les aborigènes décident donc judicieusement de construire eux aussi des tours de
contrôle en bois pour faire tomber du ciel des caisses de nourriture. Or ces êtres simples et bêtes ne réalisent qu'il
ne suffit pas de copier en apparence les techniques pour en récolter les bienfaits.

On passe assez vite sur la logique colonialiste "les aborigènes sont des gens débiles" et le fait que cette histoire
tient plus probablement de la légende urbaine qu'autre chose, pour se recentrer sur l'objectif. Si ton client a l'idée
de faire la même chose que la concurrence, alors il se trompe probablement parce qu'il devrait faire ce que toi tu lui
dis de faire avant ça. L'idéal est de saper toute velléité d'innovation qui ne t'arrange pas.

Est-ce que toi en tant que consultant ton business serait pas d'appliquer du culte du cargo à toutes les sauces chez
tes clients ? On a pas le temps pour l'introspection, le but c'est de justifier ton TJM, pas de douter de ta posture.

# Les lois chimiques

La chimie traitant d'évolution, de mélange, de changement, c'est une source inépuisable de métaphores ineptes et
de poncifs, n'hésitez pas à replonger dans vos cours de collège.

## Loi des gaz

La loi des gaz nous dit qu'un gaz remplit l'espace qui le contient, c'est l'autre nom de la loi de Parkinson.
Petit problème : le nom "Loi des gaz" fait un peu loi-inventée-à-la-volée. Dans le doute, utilisez plutôt la "Loi des
gaz parfaits", si votre interlocuteurs a de la mémoire mais pas trop, il se rappellera que cette loi somme toute
naturelle est réelle, et en plus vous passerez pour un curieux de la chimie.

Bon par contre, la loi des gaz parfaits ne veut pas dire ça du tout (c'est PV=nrT), mais l'on ne s'encombre
pas de la vérité quand on veut écraser ses interlocuteurs de sa puissance intellectuelle.


## Principe du Chatelier

>Lorsque les modifications extérieures apportées à un système physico-chimique en équilibre provoquent
une évolution vers un nouvel état d'équilibre, l'évolution s'oppose aux perturbations qui l'ont engendrée
et en modère l'effet.

Le système réagit toujours négativement à toute volonté de changement, à dire quand on essaye des trucs qui ne
changent rien dans une équipe.

# Conclusion

Quand tu sais pas grand chose, l'important c'est de le dire en étant assertif, c'est le principe du
consultant. Pour ça, connaître quelques lois générales et inutiles sont toujours utiles pour impressionner ton auditoire.

Pour finir, la dernière loi :

### Loi de Fabinout

> Pour étaler ta connaissance, il faut être convaincu de ce que tu racontes, quitte à inventer des lois qui n'existent pas.








