---
title:  "Quels outils pour gérer la connaissance dans son entreprise"
---

# Quels outils pour gérer la connaissance dans son entreprise (Knowledge management aka KM)

Gérer la connaissance dans une entreprise est toujours une gageure. Cette tache rébarbatrice de documentation est toujours reléguée aux calendes grecques. Jusqu'au jour ou le départ d'un collaborateur vous rappelle a l'ordre.

Du coup la question se pose. Quel outil pour gérer sa connaissance ? Des fichiers words dans un Filesystem ? Un google drive ? Une solution SaaS ? Un wiki hébergé.

Plutôt que de poser les élements de l'analyse à votre place (je ne connais pas les contraintes de votre organisation),
je vais vous dire ce que nous avons fait.


## Les solutions non retenues.

Tout d'abord les perdants. Nous avons fait l'impasse sur la solution du filesysteme. Nos clients travaillent en depuis des pays différents et n'ont pas de WAN. De plus, à l'heure de SaaS ca fait un peu viellot...

Nous n'avons pas retenu non plus la solution d'un Drive ou autre solution de stockage cloud. Pour des raisons de performance de recherche, de versionning et de facilité d'accès à l'information.



## Nos deux solutions pour un outil de KM

Nous avons shortlisté donc deux solutions.

1. Une solution de KM en SaaS
2. Une soluton de KM en self hosted (plusieurs choix)


### Solution SaaS

une solution en SaaS est l'option la plus pratique et la plus facile à mettre en oeuvre. Rapide à mettre en oeuvre, elle permet de se lancer sans trop se poser de question.
Après une rapide recherche, la solution qui revient le plus souvent est **Confluence** de Altassian. C'est une solution mature et performante.
Les prix sont assez abordables pour les equipes de max 10 personnes.

https://fr.atlassian.com/software/confluence/pricing?tab=cloud

Attention par contre, confluence à un coté piegeux, dans le sens ou le jour ou vous aurez besoin de plus de 10 utilisateurs, vous aurez probablement tellement de contenu dans Confluence qu'il sera quasi impossible de partir...

#### pros

- Rapide à mettre en oeuvre
- Simple à appréhender
- Disponible
- Pas de maintenance (pas de serveur à installer et à maintenir)
- Support exceptionnel

#### cons

- Cout.
- Absence de controle sur les données.
- explosion des couts avec l'augmentation de la taille de l'équipe.


### Solution self Hosted (gratuites)

Les solutions en self hosted sont celles vers lesquelles vous allez vous orienter si vous ne souhaitez pas payer, ou si vous voulez garder vos données chez vous.
Nous avons identifiées plusieurs qui peuvent convenir. La plus utilisée est sans doute **xwiki** qui est un KM avec toutes les fonctionnalités qu'on peut attendre d'un outil de KM (arborescence, recherche, import de documents word...).

En voici quelques autres

["Bookstack"](https://www.bookstackapp.com)
["Tiddlywiki"](http://tiddlywiki.com/)
["Xwiki"](http://www.xwiki.com/fr)
["Documize"](https://github.com/documize/community)



#### pros

- Gratuit
- Controle sur les données

#### cons

- Maintenance (Serveur a mettre en place + administration)
- Risque de perte de données en cas de panne
- Plus long à mettre en place.


## Conclusion

Dans notre cas, nous avons choisi de partir sur confluence, afin de ne pas perdre de temps et d'avoir l'esprit tranquille.

