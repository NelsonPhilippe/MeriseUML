# MeriseUML

## Table des matière 

- [Introduction](#Introduction)
- [Diagrammes de cas d'utilisations](#Diagrammes-de-cas-d'utilisations)
- [Maquette](#maquette)
- [Diagrammes d'états](#diagramme-détats)
- [Diagrammes d'activités](#diagrammes-dactivités)
- [Diagrammes de séquences](#diagrammes-de-séquences)

## Introduction

L'UML (Unit Modelisation Language) est un language de modelisation


Maquette
Diagrammes d'états 
Diagrammes d'activités
Diagrammes de sequences


## Diagrammes de cas d'utilisations

Le diagrammes de cas d'utilisations permet de modéliser les actions que pourra efféctuer un utilisateur, c'est un scenario qui décrit l'ensemble des interactions possible entre l'utilisateur et la machine. <br>

Le diagramme de cas d'utilisations est composée de plusieurs élements, celui ci peut contenir un système, celui ci est représenté par un cadre contenant un titre.
Il doit contenir un ou plusieurs acteurs. Il existe 2 types d'acteurs, ils sont repérés par leur positions par rapport au système.
> L'acteur principale ce trouve à gauche du diagramme, et l'acteur secondaire a droite.
> L'acteur principale initie le cas d'utilisation, il s'agit donc du système, nous nous appuyons sur d'autre acteurs pour récupérer d'autres informations, ceux si ont invoqué par les différents cas d'utilisations.

Dans le diagrammes d'utilisations nous relions les acteurs avec des cas d'utilisations avec un flèche ayant une pointe triangulaire pleine.
Nous pouvons aussi faire hériter des acteurs de certains cas d'utilisation en les reliant avec une fèche ayant une pointe triangulaire vide, ils pourront donc utiliser les actions aue peuvent effectuer une acteur.

Nous pouvons aussi creer des relations d'inclusions, en nous servant du terme "include".
Cette relation est donc représenté par une flèche en pointier et une point de flèche pleine, au centre de cette flèche il doit y être écrit "include".
Cette relation nous permet de des cas d'utilisations obligatoires pour que le programme puisse continuer de fonctionnner.

Il est aussi possible de creer des relations de possibilité, en nous servant du terme "extends".
Il devient donc optionnel d'effectuer les actions reliés par cette flèche, elle représenté de la même façon que la relation d'inclusion en remplaçant "include" par "extends".

Le diagramme permet de visualiser le comportement d'une application global mais il manque certaine informations que nous pouvons renseigner grâce au complément textuel. UML ne définit pas de conventions sur ce complement d'informations.

## Maquette

Il existe plusieurs étapes avant de commencer a construire une maquette, le Zoning et le Wireframe, nous ne pouvons pas commencer à déssiner avant ces étapes, il faut d'abord mettre en place une ergonomie optimal avant de vouloir faire le visuel de l'application.

### Le zoning

Le zoning est mise en page grossière de l'application, elle ne respecte pas forcement les propotions, le minimum d'information doit apparaître. Le but du zoning est de montrer les fonctionnalités principales et les zones principales de l'applications.

### Wireframe

Le warframe vient completer le zoning, les blocs définient auparavant par le zoning seront complété par des élements (textes, images...), nous parlons ici de positionnement des différents éléments, mais atentions le wireframe ne doit pas être détourné de ça fonctionnalité principale, il doit pouvoir nous donner une visualisation global de l'ergonomie de l'application.
Les wireframes sont souvent monocromes et écrit à la main.

### Le mockup

le mockup est la troisième étape du maquettage d'une application, il va transformer la wireframe pour avoir une représentation final du programme, il faut donc ajouter les différents images, couleurs...

### Le prototypage 

Le prototypage permet de rendre le mockup dynamique et fonctionnel, il n'est pas déstiné au développeur mais au potentielle client pour vendre une application.

## Diagramme d'états

Le digrammes d'états (state diagramme) ou digrammes d'états transitionnels définis le comportements d'un automate, il va définir un comportement fix c'est à dire une série d'actions prédéterminées.

Il est représenté par différents états : 

- Un états initial.
- Un états final.
- Entre deux états, une succession d'états intermédiaires.
- Chaque états lié par des transitions.
- L'état final est parfois absent. Il ce peut que un automate ne s'arrête jamais.

## Diagrammes d'activités

Le digrammes d'activités décris la méthode, le processus d'un cas d'utilisation. Il décrit comment est réalisé l'application contrairement au diagrammes d'états qui lui va décrire ce que fait l'application. Ce diagramme ce rapproche a de l'algorithme il serai facile de générer du code à partir de celui-ci.

La forme de ce diagramme est très similaire au diagramme d'états dans ça forme, il utilise les même comvention d'écriture.

## Diagrammes de séquences

Le diagrammes de séquences permet de visualiser une ligne temporelle d'execution de l'application, en effet, les messages ne partent pas forcement au même moment, ils ont un ordre bien précis, ils ne sont pas non plus actif au même instant.

Grâce au diagramme de séquence nous pourrons avoir un point de vue global sur l'execution, sans pour autant détailler chaque composant.

Ce diagrammes est composant de plusieurs élements : 

- Les objets : les objets sont ceux qui agissent, ils font démarrer la séquence.
- Les messages : les messages sont envoyés entre les différents objet, ils peuvent être envoyé de façon synchrone ou asynchrone. Il peut éffectuer plusieurs actions (contenu, invocation d'une méthode, création et suppression d'un objet).
- Les fragments de séquences : regroupement logique représenté par un rectangle, ils permettent de creer des structures conditionnels et des boucles. Ils contiennent des opérendes d'intéractions défini par un opérateur d'intéraction.

