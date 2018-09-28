# L'indexation sémantique

## Principes de base

### Ingénierie des connaissances et Web sémantique

L’[`ingénierie des connaissances`](https://mnemotix.gitbook.io/weever/en-savoir-plus/definitions#ingenierie-des-connaissances-ic), issue de l’[`intelligence artificielle`](https://mnemotix.gitbook.io/weever/en-savoir-plus/definitions#intelligence-artificielle-ia) \([IA](https://afia.asso.fr/wp-content/uploads/2015/06/diamant-2018-1.png)\) a pour vocation d’extraire la connaissance \(individuelle ou collective, explicite ou implicite, stabilisée ou évolutive, experte ou technique,...\) et de la modéliser dans des formalismes interprétables par des machines \(cette formalisation des connaissances d'un domaine est aussi appelée [`ontologie`](https://mnemotix.gitbook.io/weever/en-savoir-plus/definitions#ontologie)\). Cette discipline est au cœur du Web de données et propose un modèle commun de représentation permettant le partage, la réutilisation et l'interopérabilité des données du web comme des données d’entreprises.

Le **Web de données** met en relation d'immenses sources de données et offre ainsi à ceux qui savent l’exploiter une information riche et structurée, réutilisable et disponible gratuitement sur le Web dans des formats standards.

Le [`Web sémantique`](https://mnemotix.gitbook.io/weever/en-savoir-plus/definitions#web-semantique) favorise quant à lui le déploiement de techniques innovantes permettant aux applications d’utiliser plus efficacement les données. La valeur ajoutée par la sémantique est considérable au regard des services qu’il est possible de construire en les liant aux richesses disponibles sur le web des [`données ouvertes liées`](https://mnemotix.gitbook.io/weever/en-savoir-plus/definitions#donnees-ouvertes-liees) \([Linked Open Data](https://fr.wikipedia.org/wiki/Linked_open_data)\).

![Passer d&apos;un web de documents &#xE0; un web de donn&#xE9;es](https://lh3.googleusercontent.com/QzSwD5keFGIHjJu7gFdkeDsqUhq1AS8kQbhGSvZWVri3MwExkUKdWnjkoIOIblcaoIb4lU4Fa0w1Gibk3zBqK9P7xWn5qoxK39uRPPT6AQFqxn7zoCbKrJkgyTNsgOV8uKe-_3LupL4)

{% hint style="info" %}
**"Suppose I could program my computer to create a space in which anything could be linked to anything"**  - [Tim Berners-Lee](https://fr.wikipedia.org/wiki/Tim_Berners-Lee) \(fondateur du web - 1990\)
{% endhint %}

### Enrichissement des données et indexation sémantique

Le nom Weever fait référence au livre écrit par Tim Berners-Lee \("[Weaving the Web](https://www.w3.org/People/Berners-Lee/Weaving/Overview.html)"\) et à l'action de **tisser les ressources entre elles**. Weever implémente des technologies sémantiques issues de l'ingénierie des connaissances, pour tisser des liens dans des données qui n'en ont pas, ce qui revient à les enrichir considérablement.

![](../.gitbook/assets/image%20%2857%29.png)

Weever réalise de façon quasi automatique une **indexation sémantique**, qui consiste, lors de l’analyse de tout élément versé dans l'archive Weever, à rattacher chaque mot à un concept sous-jacent. Les thésaurus de **Koncept** \(notre outil de gestion collaborative de terminologies\) sont intégrés dans Weever pour aider à indexer les ressources \(événements, mémos, personnes, œuvres, projets, images, fichiers...\). 

![Int&#xE9;gration des branches du th&#xE9;saurus dans le tagging de concepts de tous les &#xE9;l&#xE9;ments de Weever](../.gitbook/assets/image%20%2834%29.png)

Comme le [`thésaurus`](https://mnemotix.gitbook.io/weever/en-savoir-plus/definitions#thesaurus) est construit en respectant les standards du web sémantique, il permet d'aller plus loin qu'un simple tagging de folksonomie, puisque les tags/concepts sont structurés et agencés dans une représentation hiérarchique : 

![Du nuage de mots &#xE0; la structuration de concepts dans un th&#xE9;saurus](../.gitbook/assets/image%20%2816%29.png)

Dans nos applications Weever et Koncept, nous utilisons le format [SKOS](http://www.ala.org/alcts/resources/z687/skos) \(« système simple d'organisation des connaissances »\), recommandé par l'instance normative du Web le [W3C](https://www.w3.org/), pour représenter les thésaurus, les classifications ou d'autres types de vocabulaires contrôlés. "S'appuyant sur le modèle de données [`RDF`](https://mnemotix.gitbook.io/weever/en-savoir-plus/definitions#rdf-rdfs-owl), son principal objectif est de permettre la publication facile de vocabulaires structurés pour leur utilisation dans le cadre du Web sémantique" \(source [Wikipédia](https://fr.wikipedia.org/wiki/Simple_Knowledge_Organization_System)\). 

La figure ci-dessous illustre cette représentation hiérarchique sur le concept "Chat" détaillant les relations génériques \(_broader_\), spécifiques \(_narrower_\) ou reliées \(_related_\) avec d'autres concepts et dont l'illustration forme un graphe :

![](../.gitbook/assets/image%20%2860%29.png)

### Le reconnaissance de concepts

Pour faciliter la tâche d’annotation et d’enrichissement des données, nous avons développé un algorithme innovant de détection sémantique de concepts permettant d’annoter automatiquement ou d’assister l’annotation manuelle d’un texte avec les concepts du thésaurus et de l'ontologie structurant Weever.

![Processus de d&#xE9;tection des concepts dans un texte](../.gitbook/assets/image%20%2852%29.png)

## L'indexation sémantique semi-automatique

Nous expliquons dans ce paragraphe le processus innovant de détection semi-automatique de concepts réalisé dans Weever.

Tous les éléments de Weever, soit les profils, les projets, les événements et les ressources ont dans leur onglet Paramètres l'intégration du \(ou des\) thésaurus de Koncept dans la colonne de droite. Cet intégration permet de sélectionner des concepts pour indexer au mieux l'élément. 

![Int&#xE9;gration du th&#xE9;saurus dans tous les &#xE9;l&#xE9;ments de Weever](../.gitbook/assets/index.png)

Outre cette possibilité de taguer soi-même les éléments, Weever propose aussi des suggestions de concepts \(en fonction des textes de description, des autres éléments tagués dans le projet comme les ressources etc...\), pour aider l'utilisateur à mieux indexer les éléments dans Weever.

### Suggestion de concepts

La figure ci-dessous montre comment Weever propose une suggestion de concept dans une des branches du/des thésaurus. Le concept suggéré est grisé, il suffit de cliquer dessus pour accepter qu'il soit utilisé : 

![Suggestion de concept](../.gitbook/assets/image%20%2862%29.png)

Une fois validé, le concept change de couleur \(celle de la branche à laquelle il appartient\) : 

![Validation de concept](../.gitbook/assets/image%20%2831%29.png)

{% hint style="success" %}
**La détection automatique de concepts marche aussi à l'import de nouvelles ressources textuelles comme du texte, word, odt ou pdf**
{% endhint %}

### Aide à une meilleure indexation

Concernant les ressources, dans la liste des ressources, un petit icône de warning a été placé dans la rubrique Statut pour attirer l'attention sur le fait que la ressource n'a pas été suffisamment documentée \(pas de titre, pas légende, pas de concept associé\). Ce n'est pas obligatoire, cependant, c'est toujours mieux pour exploiter par la suite les données de l’archive.

![](../.gitbook/assets/image%20%2826%29.png)

