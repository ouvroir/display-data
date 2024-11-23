# Data for Display

Ce dépôt contient des descriptions d’expositions qui servent de jeux d’essai dans le cadre des expérimentations menées pour le projet [Display](https://github.com/ouvroir/display/).

L’ontologie utilisée est disponible à cette adresse : [https://github.com/ouvroir/display/](https://github.com/ouvroir/display/).

# Objectif de l’encodage

- mettre à l’épreuve Display Ontology par la description d’expositions
- tester le potentiel d’inférer des relations topologiques

# Travaux

## En cours

- Feux pâles

## À venir

- décrire une exposition à partir d’une documentation lacunaire
- décrire un cas limite

# Recommandations

Cette section détaille les conventions d’encodage suggérées dans le contexte des expérimentations en cours.

## Renseigner systématiquement la propriété `rdfs:label`

Peu d’information sur les expôts est actuellement disponible dans ce jeu de données : la description de l’exposition est circonscrite par les relations topologiques. Dans ce contexte, `rdfs:label` est utilisé fournir des éléments d’information interne permettant de repérer une ressource sur le plan. Il s’agit de créer un lien informel entre les ressources (au sens de RDF) et les informations documentaires utilisées.

Référence : [Label Everything](https://patterns.dataincubator.org/book/label-everything.html)

Remarque : l’utilisation de deux propriétés `rdfs:label` ou plus pour une même entité, par exemple avec différentes étiquettes linguistiques, rend les données non conformes au modèle de Linked Art.

Référence : [core-properties](https://linked.art/model/base/#core-properties)

## Identifier les ressources selon la convention proposée

- `exhib:space[0-9]{4}`
- `exhib:exhibit[0-9]{4}`
- `exhib:element[0-9]{4}`

`[0-9]{4}` est un numéro séquentiel unique qui commence à `0000` pour chacun des trois types de ressources. Exemple : 0016.

## Approche

*Décrire minimalement*

Un des objectifs de ces descriptions est d’expérimenter l’inférence des relations topologiques. Décrire la topologie des objets de façon minimale (description lacunaire), puis tenter de maximiser les inférences.

# Validation syntaxique

Copier-coller le contenu du fichier dans ce formulaire : [http://ttl.summerofcode.be](http://ttl.summerofcode.be)

Ou :

```bash
$ npm install -g turtle-validator
```

puis

```bash
$ ttl <path-to-file ...>
```

Informations :

- https://github.com/IDLabResearch/TurtleValidator

# Notes sur les inférences

À venir