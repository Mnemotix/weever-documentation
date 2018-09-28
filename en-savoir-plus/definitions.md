# Définitions

## Ingénierie des connaissances \(IC\)

l’Ingénierie des Connaissances, elle-même sous branche de l'Intelligence Artificielle, est une des dimensions de la gestion des connaissances au sein d'une organisation. Elle fait référence à l'ingénierie des systèmes complexes « intelligents » incorporant beaucoup de connaissances tels que les systèmes experts.

## Web sémantique

Il favorise le déploiement de nouvelles techniques permettant aux applications d’utiliser plus efficacement les données en reconnaissant les différents types de ressources et de liens qu’elles rencontrent sur le web, et en exploitant le sens et les raisonnements qui leur sont attachés. Ces technologies permettent d’ajouter des métadonnées à n’importe quelle ressource Web de manière à la décrire plus finement que ce que permet le HTML basique. Ces métadonnées sont directement issues d’un travail de modélisation en amont d’un domaine de connaissance \(mode, arts, sciences, etc\) à travers un document appelé ontologie ou thésaurus.

## Intelligence Artificielle \(IA\)

L’Intelligence Artificielle est un domaine vaste et pluridisciplinaire dont l’unité tient dans l’ambition initiale de faire reproduire par les machines des compétences cognitives qui sont normalement l’apanage de l’être humain : perception de l’environnement, représentation conceptuelle du monde, pensée, raisonnement, décision pour action \(aller plus loin : [https://recherche.orange.com/lintelligence-artificielle-expliquee-aux-humains/](https://recherche.orange.com/lintelligence-artificielle-expliquee-aux-humains/)\).

## Métadonnées

Généralement définies comme “données sur les données” ou “information sur les données”. Les métadonnées sont une liste structurée d’information qui décrivent les données ou les services \(incluant les données numériques ou non\) stockés dans les systèmes d’information. Elles peuvent ainsi contenir une brève description sur le contenu, les objectifs, la qualité et la localisation de la donnée, comme des informations liées à sa création.

## Ontologie

Une ontologie est un ensemble de concepts et de relations modélisant un domaine de la connaissance sans ambiguïté. La représentation d’une ontologie dans un langage formel \(obéissant à une logique stricte\) permet à un ordinateur d’exploiter les connaissances modélisées. L’ontologie est la forme la plus aboutie \(et aussi la plus complexe\) de la modélisation sémantique alors que le thésaurus est un outil plus simple connu depuis longtemps par les professionnels de la documentation \(archivistes, documentalistes, bibliothécaires, ...\). Pour aller plus loin voir le diaporama : [Donner du sens à des documents numériques : potentiel des ontologies et du web sémantique](https://f-origin.hypotheses.org/wp-content/blogs.dir/2791/files/2016/03/29160324_aussenac_diaporama.pdf).

## Thésaurus

Un thésaurus \(autrement appelé thésaurus de descripteurs ou thésaurus documentaire\), est une liste organisée de termes contrôlés et normalisés \(descripteurs et non descripteurs\) représentant les concepts d'un domaine de la connaissance. C'est un langage contrôlé utilisé pour l'indexation de documents et la recherche de ressources documentaires dans des applications informatiques spécialisées.

## RDF/RDFS/OWL

Le W3C \(World Wide Web Consortium\) est à l’origine de la plupart des standards du Web. Il est présidé par Tim Berners Lee qui est également l’inventeur du Web sémantique. Dès 2001, le W3C a proposé un ensemble de standards pour l’écriture des données et des métadonnées du Web sémantique au format XML. RDFS et OWL sont des standards pour l’écriture des ontologies. RDFS pour les ontologies simples et OWL pour les ontologies plus avancées. RDF est le format d’échange des annotations sémantiques sur le Web, c’est à dire les données qui exploitent les ontologies.

## Données ouvertes liées

Autrement dit _Linked Open Data_ \(ou LOD\) est un concept qui associe systématiquement deux modes différents de gestion de la donnée présente sur l'Internet, c'est à dire la donnée liée \(selon les principes du web sémantique édictés par Tim Berners-Lee, le fondateur du Web\) et la donnée ouverte \( Open Data considérée comme une information publique brute qui a vocation à être librement accessible et réutilisable\).

## Plateforme web

Elle désigne un écosystème logiciel développé sur-mesure par Mnémotix pour les besoins d'un client. Fondé sur les principes du Web sémantique, cet écosystème est une architecture complexe, organisée comme un ensemble de services \(génératifs, informatifs et collaboratifs\) orchestrés par une API centrale, le middleware.

## **Middleware \(sémantique\)**

Le middleware est une couche d’abstraction qui représente l’ensemble des services logiciels qui font le ****lien entre les applications clientes \(interfaces Web, applications mobiles\) et le système de gestion et de stockage des données. Son rôle principal est de découpler les rôles concernant le développement serveur d’une part et le développement Web d’autre part. Ce découplage se manifestera par la mise en place d’un mécanisme d’interface logicielle : l’API REST.

## **API REST**

Une API REST est une interface normalisée dédiée aux développeurs d’applications Web qui leur permet par de simples requêtes HTTP d’interagir avec les objets du serveur. Une API REST doit implémenter ce qu’on appelle le CRUD \(Create, Read, Update, Delete\) pour chacun des objets du modèle. Les objets du modèle dépendent entièrement du projet, cela peut être un utilisateur, un document, un projet. Ainsi dans le cas du document, les développeurs Web savent exactement comment créer un document dans le serveur, comment le consulter, comment le supprimer, sans avoir à connaître le code côté serveur. C’est en cela qu’il s’agit d’une interface de programmation.

## Backoffice

Le Backoffice ou “interface d’administration” est une application cliente de l’API REST, le plus souvent une application Web, dont le seul rôle est de permettre aux administrateurs du système de contrôler le bon fonctionnement de l’ensemble de la solution.

## Moteur d’indexation ou moteur de recherche

C’est un élément du middleware qui prend en charge l’analyse des documents textuels \(indexation\) et qui permet par la suite de faire des recherches par mots-clés ou avec des opérateurs plus complexes.

## Moteur sémantique

Le moteur sémantique est un autre élément du middleware et qui permet d’effectuer d’autres types de recherches, non plus sur les documents mais sur les métadonnées sémantiques. C’est un élément qui charge l’ontologie de la plateforme au démarrage et qu’on peut interroger par la suite grâce au langage SPARQL qui est le langage de requête standard du Web de sémantique.

## Triple store

Le Triple Store est une base de données particulière dont le rôle est de stocker de manière efficace les métadonnées sémantiques de la plateforme.

## SPARQL Endpoint

SPARQL est le langage de requête officiel du Web sémantique. Il a été standardisé par le W3C au même titre que RDF. Ce langage sert à interroger les moteurs sémantiques \(également appelés interpréteurs SPARQL\). Un SPARQL Endpoint désigne un service particulier de l’API REST qui permet d’envoyer des requêtes SPARQL au moteur sémantique afin de récupérer des données RDF. Ce service peut être ouvert sur le Web extérieur et ainsi faire que les données dans Weever soient disponibles sur le Web de données.

