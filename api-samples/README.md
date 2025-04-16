---
title: "Display : exemples de données"
author: ouvroir
---

# Notes

Les IRI des ressources RDF, lorsque renvoyées comme valeur des champs, sont des identifiants non déréférençables (pour la majorité). Les IRI de l’espace de nom https://ouvroir.umontreal.ca avec le chemin /data peuvent être utilisées dans les requêtes à l’API.

# 001-exhibitions.json

Liste des expositions.

/apis/display/query?id=exhibitions

Il n’y a qu’une seule exposition actuellement (https://ouvroir.umontreal.ca/data/activity0000).

Format SPARQL 1.1 Query Results JSON Format (https://www.w3.org/TR/sparql11-results-json/)

# 002-exhibition.json

Description d’une exposition.

/apis/display/resource?id=exhibition&iri=https://ouvroir.umontreal.ca/data/activity0000

Description d’une exposition.

Voir la propriété `used_specific_object` pour la liste des ensembles d’exhibits utilisés par l’exposition décrite. Exemple d’un ensemble : https://ouvroir.umontreal.ca/data/set0000

# 003-ensemble-exhibits.json

Description d’un ensemble d’exhibit

/apis/display/resource?id=exhibitsSet&iri=https://ouvroir.umontreal.ca/data/set0000

Voir la propriété `member` pour la liste des exhibits membres de cet ensemble. Exemple d’exhibit : https://ouvroir.umontreal.ca/data/exhibit0015

# 004-exhibit.json, 005-exhibit.json

Exemples de description d’un exhibit (avec relations topologiques génériques).

/apis/display/resource?id=exhibit&iri=https://ouvroir.umontreal.ca/data/exhibit0015

/apis/display/resource?id=exhibit&iri=https://ouvroir.umontreal.ca/data/exhibit0006

Pour un exemple de description d’un exhibit avec ses relations topologiques spécifiques, voir l’exemple `009-exhibit-relations-specifiques.json`.

# 006-exhibition-spaces.json

Liste des espaces d’une exposition (utiliser IRI d’une exposition).

/apis/display/resource?id=exhibitionSpaces&iri=https://ouvroir.umontreal.ca/data/activity0000

# 007-space.json, 008-space.json

Exemples de description d’un espace d’exposition.

/apis/display/resource?id=space&iri=https://ouvroir.umontreal.ca/data/space0001

/apis/display/resource?id=space&iri=https://ouvroir.umontreal.ca/data/space0000

# 009-exhibit-relations-specifiques.json

Pour un exhibit, la liste des relations topologiques spécifiques. Les relations topologiques spécifiques sont des sous-propriétés de la relation topologique générique donnée par les exemples 004 et 005.

/apis/display/query?id=exhibitWithSpecificRelations&iri=https://ouvroir.umontreal.ca/data/exhibit0006

Format SPARQL 1.1 Query Results JSON Format (https://www.w3.org/TR/sparql11-results-json/)