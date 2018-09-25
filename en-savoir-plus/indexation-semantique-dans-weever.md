# Indexation sémantique dans Weever

## Principes de base

### Ingénierie des connaissances et Web sémantique

L’**ingénierie des connaissances**, issue de l’[intelligence artificielle](https://afia.asso.fr/wp-content/uploads/2015/06/diamant-2018-1.png) \(IA\) a pour vocation d’extraire l’expertise et de la modéliser dans des formalismes interprétables par des machines \(cette formalisation des connaissances d'un domaine est aussi appelée [ontologie](https://f-origin.hypotheses.org/wp-content/blogs.dir/2791/files/2016/03/29160324_aussenac_diaporama.pdf)\). Cette discipline est au cœur du Web de données et propose un modèle commun de représentation permettant le partage, la réutilisation et l'interopérabilité des données du web comme des données d’entreprises.

Le **Web de données** met en relation d'immenses sources de données et offre ainsi à ceux qui savent l’exploiter une information riche et structurée, réutilisable et disponible gratuitement sur le Web dans des formats standards.

Le **Web sémantique** favorise quant à lui le déploiement de techniques innovantes permettant aux applications d’utiliser plus efficacement les données. La valeur ajoutée par la sémantique est considérable au regard des services qu’il est possible de construire en les liant aux richesses disponibles sur le web des données ouvertes liées \([Linked Open Data](https://fr.wikipedia.org/wiki/Linked_open_data)\).

### Enrichissement des données et indexation sémantique

Le nom Weever fait référence au livre écrit par Tim Berners-Lee \("[Weaving the Web](https://www.w3.org/People/Berners-Lee/Weaving/Overview.html)"\) et à l'action de tisser les ressources entre elles. Weever implémente des technologies sémantiques issues de l'ingénierie des connaissances, pour enrichir les données traitées.

![](../.gitbook/assets/image%20%2850%29.png)

Weever réalise de façon quasi automatique une **indexation sémantique**, qui consiste, lors de l’analyse de tout élément versé dans l'archive Weever, à rattacher chaque mot à un concept sous-jacent. Les thésaurus de **Koncept** sont intégrés dans Weever pour aider à indexer les ressources \(événements, mémos, personnes, œuvres, projets, images, fichiers...\). 

![Int&#xE9;gration des branches du th&#xE9;saurus dans le tagging de concepts de tous les &#xE9;l&#xE9;ments de Weever](../.gitbook/assets/image%20%2830%29.png)

Comme le thésaurus est construit en respectant les standards du web sémantique, il permet d'aller plus loin qu'un simple tagging de folksonomie, puisque les tags/concepts sont structurés et agencés dans une représentation hiérarchique \(notamment par l'usage de vocabulaires contrôlés basés sur le système [SKOS](http://www.ala.org/alcts/resources/z687/skos)\).

![](../.gitbook/assets/image%20%281%29.png)

## L'indexation sémantique semi-automatique



Le petit icône de warning a été placé dans la rubrique Statut pour attirer l'attention sur le fait que la ressource n'a pas été suffisamment documentée \(pas de titre, pas légende, pas de concept associé\). Ce n'est pas obligatoire, cependant, c'est toujours mieux pour exploiter par la suite les données de l’archive.  


![](../.gitbook/assets/image%20%2824%29.png)

