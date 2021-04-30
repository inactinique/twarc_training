# Premières requêtes avec twarc

L'installation de twarc permet l'usage de deux commandes distinctes: twarc et twarc2. `twarc`utilisera l'API v1.1 et `twarc2`qui permet d'interagir avec l'API v2. 

## Configurer twarc

Il faut avoir à disposition le bearer token.

`twarc2 configure`

Rentrer le token.

Éventuellement, donner les éléments de configuration supplémentaires demandés, qui sont facultatifs (et ne nous concernent pas pour cette formation).

## Première requête

Dans un terminal (Terminal.app sous macOS, Terminal sous linux, ... sous Windows), entrer:

`twarc2 search 'votremotclé' --limit=1000 > votremotclé.json`

On limite ici la requête à 1000 tweets, pour ne pas diminuer trop notre quota mensuel de tweets.

puis

`twarc-csv votremotclé.json > votremotcle.csv`

votremotclé.csv sera ouvrable par un tableur (excel, calc, etc). Attention, conservez le json à titre d'archive. Le format json, mieux structuré que le csv, est plus approprié pour une conservation / archivage de vos données.

Ouvrons le fichier votremotclé.csv. Regardez les dates. Que constatez-vous?

## Chercher dans l'historique des tweets

Nous allons maintenant faire notre première requête fouillant dans l'historique des tweets au-delà d'une semaine.

`twarc2 search --archive 'votremotclé' --limit=1000 --start-time 2018-01-01 --end-time 2018-12-31 > votremotclé.json`


[<<< Retour](04CreerAppTwitter.md)
