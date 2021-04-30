# Les possibilités de l'API de Twitter

## API: définition rapide

Une interface de programmation applicative  (Application Programming Interface - API) est un dispositif logiciel permettant à deux programmes de communiquer des fonctionnalités ou des données par exemples / façade permettant à un logiciel (dont les sites web) d'offrir des services à d'autres  logiciels. (https://fr.wikipedia.org/wiki/Interface_de_programmation)

## L'API de Twitter

Twitter a toujours eu une API permettant des collectes de données assez importantes, mais aussi des partages de fonctionnalités (les boutons type « partage sur Twitter » mais aussi la possibilité à partir d'une application ou d'un site web de publier un tweet au nom d'un utilisateur par exemple).

Nous intéresse ici la possibilité de collecter des données via l'API de Twitter. Cette API donait jusqu'à présent (versions 1 puis 1.1) en gros trois possibilités de collecter des données:

- La recherche dans l'historique des tweets: sur une semaine dans le passé, jusqu'à 3000 tweets environ par heure;
- La collecte du stream de tweets, soit jusqu'à 1% des tweets publiés, calculé par 1/4 d'heure;
- L'accès payant à l'ensemble de Twitter.

## Quelques outils utilisables jusqu'ici

Différents types d'authentification sont possibles, avec pour résultat concret:

- de pouvoir utiliser la recherche dans l'historique sans compte développeur avec un logiciel comme [TAGS](https://tags.hawksey.info/)
- de pouvoir capturer un stream de tweets avec un logiciel comme [DMI-TCAT](https://wiki.digitalmethods.net/Dmi/ToolDmiTcat)
- de contourner la limitation -- MAIS SANS RESPECT DES TOS DE TWITTER -- de l'API Search avec des outils comme [twint](https://github.com/twintproject)

Attention, l'utilisation d'outils respectant les terms of usage (TOS) de Twitter n'impliquent pas d'être en conformité avec le RGPD. Cette dernière nécessite de se rapprocher des responsables CNIL / DPO de vos institutions.

## Les nouveautés de l'API v2

Pour le moment, la version de l'API de Twitter qui reste valable est le 1.1. La v2 la remplacera à un horizon non encore déterminé. La grande nouveauté, pour les chercheurs et chercheuses de la v2 est la possibilité d'y demander accès en tant que chercheur / chercheuse et d'avoir un accès nettement plus large à l'historique des tweets: on passe de 3000 tweets par heure sur 7 jours max à 10 millions de tweets sur l'ensemble de l'historique de Twitter ([Academic Research Product Track](https://developer.twitter.com/en/solutions/academic-research/products-for-researchers)). Par contre, l'accès au stream semble plus restreint qu'avec la v1.1.

## twarc

Pendant cette formation, nous allons utiliser l'ensemble d'outils que constitue twarc. 

Petit historique de twarc: le nom 'twarc' est la contraction de 'tweet' et 'archives'. Le logiciel répond au besoin de documenter les événements du présent pour études futures. Il est né de la coopération entre des développeurs et des universitaires lors des émeutes de Ferguson et de la naissance du mouvement (et hashtag) Black Lives Matter.

Les conditions de sa naissance assurent un certain nombre d'avantages: souci de l'éthique, respect des mouvements activistes, respect des conditions juridiques mises au point par Twitter, mais aussi d'un certain nombre de contraintes techniques de l'API de Twitter (nombre de requêtes autorisées par exemple).

Un autre avantage est aussi que twarc gère les deux version de l'API, la v1.1 amenée à disparaître, la v2 amenée à se développer. Développé par des universitaires, twarc a été l'un des premiers outils à pouvoir utiliser cette nouvelle possibilité offerte par Twitter aux chercheurs et chercheuses.

Twarc a mené à un projet plus vaste dont il est maintenant une partie, Documenting the Now (DocNow), coopération entre l'université du Maryland, l'Université de Virginie, le [Shift collective](https://www.shiftcollective.us/) et la fondation A. Mellon. Consulter le site de [DocNow](https://www.docnow.io/) est intéressant, car d'autres outils que twarc y sont proposés. Le site renvoit notamment à un meta-catalogue de corpus de tweets.

[Suite >>>](02PreRequis.md)
