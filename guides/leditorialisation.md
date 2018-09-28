# L'éditorialisation

Les applications de [Mnémotix](http://www.mnemotix.com/) comme Weever \(et sa version mobile\) et Koncept reposent sur un socle technologique souple, modulaire et open source : notre middleware sémantique Synaptix \(voir le chapitre **En savoir plus /** Le middleware Synaptix\).

Weever et Koncept sont à considérer comme des solutions de backoffice destinées à une communauté "d'experts" dans le but de constituer et d'alimenter leur base de connaissances. 

![](../.gitbook/assets/image%20%2828%29.png)

Pour avoir accès publiquement, c'est à dire sur le web, aux informations enrichies par les algorithmes sémantiques de Synaptix, nous proposons plusieurs solutions **d'éditorialisation** des données : 

* exporter les données au format Linked Open Data \(JSON, XML, RDF...\)
* passer par notre API REST \(pour interroger programmatiquement le cœur de Synaptix et construire des plugins à façon\). Nous avons déjà réalisé un connecteur pour le CMS Drupal et pour Wordpress \(en cours\)
* mettre à disposition un SPARQL Endpoint pour interfacer les données enrichies avec les standards du web sémantique
* créer des exports pour générer des sites web à façon

Nous présentons ci-dessous un exemple d'éditorialisation exportant des données de Weever vers un site web public, celui de la Fondation [Lafayette Anticipations](https://lafayetteanticipations.com/fr). Les données du profil de l'artiste servent à alimenter sa fiche de présentation sur le site Drupal public.

![](../.gitbook/assets/image%20%2840%29.png)

