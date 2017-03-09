#  Le succès d'AlphaGo contre l'humain via Deep Learning
<br />
## Introduction
Le Go est un jeu de plateau ancient pour deux joueurs et depuis longtemps il est considéré comme le jeu le plus complex inventé par l'humain. Même après avoir vu le victoire de Deep Bleu contre le champion du monde dans l'échec, on ne pense toujours pas qu'un programme peut être capable de battre l'humain dans le Go.

Pourtant AlphaGo est arrivé. Créé par l'équipe DeepMind de Google, cette intelligence artificielle a réussi à battre un des meilleurs joueurs professionnels en 2016. Cet succès donne sans doute du crédit aux méthodes de Deep Learning employées dans son algorithme et donc ma veille consiste à découvrir pourqoui on a besoins de ces outils puissants et comment ils sont appliqués.

## Le Go, un jeu ancient et complex
### Qu'est-ce que c'est ?
Le Go est un jeu de plateau originaire de Chine avec plus de deux milles ans d'histoire. 
![Image du jeu de Go](/images/Go.png)

En terme de règle :
>  Il oppose deux adversaires qui placent à tour de rôle des pierres, respectivement noires et blanches, sur les intersections d'un tablier quadrillé. Le but est de contrôler le plan de jeu en y construisant des « territoires ». Les pierres encerclées deviennent des « prisonniers », le gagnant étant le joueur ayant totalisé le plus de territoires et de prisonniers. - Wikipédia

Comparé avec l'échec, les règle du Go sont beaucoup plus simples. Pourtant le Go est toujours considéré comme un des jeux les plus complexes et personne n'a pu imaginer, avant la naissance d'AlphaGo, qu'un jour un programme peut battre l'humain dans ce jeu-là. Pourquoi ?

### La complexité du jeu


## Comment construire un algorithme de joueur ?
Le Go est un jeu à information parfaite. C'est-à-dire que toute information nécessaire pour prendre de la décision d'un tour est transparente et acccessible aux deux joueurs. Dans le cas du Go, cette information est uniquement l'état actuel du plateau. Donc, ce dernier est la seule donnée qu'on doit fournir en entrée, si on conçoit un algorithme qui joue au Go. Puis l'algorithme doit être capable de calculer en sortie une transformation à un autre état de plateau valable qui a une plus forte chance de gagner.

### Arbre de jeu
Comment ce calcul peut être réaliser ? L'idée est que si on prend l'état initial du jeu comme un noeud de racine et tous les états valables dans le tour prochain comme ses noeuds d'enfant et ainsi de suite, on peut construire un arbre qui contient tous les possibilités du jeu depuis le début jusqu'à la fin. 

[image arbre tic-tac-toe]

Un chemin depuis le noeud de racine à un noeud de feuille est alors un jeu complet. Donc, étant donné un état actuel de jeu, le calcul du programme peut être le parcours du sous-arbre partant de ce noeud actuel pour trouver un noeud d'enfant qui permet le plus de cas gagnants. Des algorithmes comme Min-Max sont en effet des réalisations concrètes de cette idée-là.

Cependant, cette approche est problématique voire même irréalisable pour le Go. 

## Problème critique pour le Go

[image arbre Go]

## Approche avant AlphaGo

## Amélioration par introduction de Deep Learning

## Quelques records

## Conclusion
