# L'éditorialisation

Les applications de [Mnémotix](http://www.mnemotix.com/) comme Weever \(et sa version mobile\) et Koncept reposent sur un socle technologique souple, modulaire et open source : notre [`middleware sémantique`](https://mnemotix.gitbook.io/weever/en-savoir-plus/definitions#middleware-semantique) Synaptix \(voir le chapitre **En savoir plus /** [Le middleware Synaptix](https://mnemotix.gitbook.io/weever/en-savoir-plus/le-middleware-synaptix)\).

Weever et Koncept sont  des solutions de documentation destinées à une communauté "d'experts" dans le but de constituer, d'alimenter et d'enrichir sémantiquement leur base de connaissances. 

![De la donn&#xE9;e enrichie &#xE0; la donn&#xE9;e publi&#xE9;e](../.gitbook/assets/image%20%2829%29.png)

Pour valoriser les données de cette base de connaissance auprès de divers publics, nous proposons plusieurs solutions **d'éditorialisation** des données : 

* exporter les données au format Linked Open Data \(JSON, XML, RDF...\)
* passer par notre [`API REST`](https://mnemotix.gitbook.io/weever/en-savoir-plus/definitions#api-rest) \(pour interroger programmatiquement le cœur de Synaptix et construire des plugins à façon\). Nous avons déjà réalisé un connecteur pour le CMS Drupal et pour Wordpress \(en cours\)
* mettre à disposition un [`SPARQL Endpoint`](https://mnemotix.gitbook.io/weever/en-savoir-plus/definitions#sparql-endpoint) pour interfacer les données enrichies avec les standards du web sémantique
* créer des exports pour générer des sites web à façon

Nous présentons ci-dessous un exemple d'éditorialisation exportant des données de Weever vers un site web public, celui de la Fondation [Lafayette Anticipations](https://lafayetteanticipations.com/fr). Les données du profil de l'artiste servent à alimenter sa fiche de présentation sur le site Drupal public.

![](../.gitbook/assets/image%20%2842%29.png)

