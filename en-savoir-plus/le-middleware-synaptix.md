# Le middleware Synaptix

Mnémotix a développé une bibliothèque d'algorithmes mutualisés dans son framework Synaptix, permettant de construire des chaînes de traitement modulaires. Synaptix fonctionne comme un middleware sémantique sous la forme d’une API REST destinée à être intégrée au cœur de tous les outils de Mnémotix.

![Cha&#xEE;ne de traitement de la donn&#xE9;e](https://lh5.googleusercontent.com/Zh--fkMi4vwiRVWHhGaIypYMpz0puxNciLcaRXzPsuzVHSp7vb4g1W38_lwps8Vw1rLHApEAGJ9E7CBVnetbSRp8TjlTTh-MQMAIoPn6Iiv1mGIncLMiaj1ERNUeEZs0L9eYxZqf)

Dans le cadre du déploiement de Synaptix, la chaîne à mettre en place est à minima constituée de : 

* Un module de stockage
* Un module d’indexation
* Un module sémantique
* Des connecteurs pour l’import et la synchronisation à des sources de données extérieures \(un connecteur par source de données\)
* Un module Web pour la consultation, la recherche et la navigation dans les données collectées 

