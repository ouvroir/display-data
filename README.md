# Data for Display

Ce dépôt contient des descriptions d'expositions qui servent de jeux d'essai dans le cadre des expérimentations menées pour le projet [Display](https://github.com/ouvroir/display/).

L'ontologie utilisée est disponible à cette adresse : [https://github.com/ouvroir/display/](https://github.com/ouvroir/display/).

# Recommandations

Cette section détaille les conventions d'encodage suggérées dans le contexte des expérimentations en cours.

## Renseigner systématiquement la propriété `rdfs:label`

Peu d'information sur les expôts est actuellement disponible dans ce jeu de données : la description de l'exposition est circonscrite par les relations topologique.
Dans ce contexte, `rdfs:label` est utilisé fournir des éléments d'information permettant de répérer une ressource sur le plan. Il s'agit de créer un lien informel entre les ressources (au sens de RDF) et les informations documentaires utilisées.

## Identifier les ressources selon la convention proposée

- `exhib:space[0-9]{4}`
- `exhib:exhibit[0-9]{4}`
- `exhib:element[0-9]{4}`

`[0-9]{4}` est un numéro séquentiel unique qui commence à `0000` pour chacun des trois types de ressources. Exemple : 0016.

# Validation syntaxique

Copier-coller le contenu du fichier dans ce formulaire : [http://ttl.summerofcode.be](http://ttl.summerofcode.be)

*Informations*

- https://github.com/IDLabResearch/TurtleValidator