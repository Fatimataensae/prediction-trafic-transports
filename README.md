# 🚆 Prédiction du trafic des transports en commun

## Présentation du projet

Ce projet de Machine Learning, réalisé en groupe dans le cadre de la Licence 3, porte sur la modélisation prédictive du trafic des transports en commun en Île-de-France à partir des données de validation des titres de transport.

L'objectif est d'exploiter les données historiques pour caractériser le niveau de fréquentation et prédire des catégories de trafic à partir de variables temporelles et des caractéristiques des validations.

## Objectifs

- Explorer et comprendre les données de validation des titres de transport.
- Préparer les données et construire des variables pertinentes pour la prédiction.
- Comparer des approches de classification supervisée.
- Évaluer les performances des modèles et analyser leurs erreurs.

## Données utilisées

Le projet s'appuie sur le jeu de données *Public Transport Traffic Data in France*, qui contient des informations sur les validations de titres de transport en Île-de-France.

Les données étudiées couvrent la période de juillet à décembre 2019.

Principales variables exploitées :
- `DATE` : date de validation ;
- `STATION_NAME` : nom de la station ;
- `TITLE_CATEGORY` : catégorie du titre de transport ;
- `NB_VALID` : nombre de validations.

## Méthodologie

1. **Analyse exploratoire** : étude des variables, de leur distribution et des données manquantes ou atypiques.
2. **Prétraitement** : nettoyage des données et préparation des variables.
3. **Feature engineering** : extraction de caractéristiques temporelles et encodage des variables catégorielles.
4. **Modélisation** : mise en œuvre d'une régression logistique multinomiale pour prédire les catégories de trafic.
5. **Évaluation** : séparation des données en ensembles d'entraînement et de test, puis analyse des performances à l'aide de plusieurs métriques de classification.

## Résultats

Sur l'ensemble de test, la régression logistique multinomiale obtient une accuracy de **74 %**.

L'analyse des performances par classe permet de nuancer ce résultat :

- **Trafic intermédiaire** : F1-score de 0,80.
- **Trafic élevé** : F1-score de 0,71.
- **Trafic faible** : F1-score de 0,44.

Ces résultats mettent en évidence des performances variables selon les catégories de trafic et soulignent l'intérêt d'analyser les erreurs de classification au-delà de l'accuracy globale.

## Technologies

- Python
- Pandas et NumPy
- Scikit-learn
- Matplotlib

## Pistes d'amélioration

- Étudier d'autres algorithmes de classification.
- Approfondir le réglage des hyperparamètres.
- Examiner le déséquilibre éventuel entre les classes.
- Explorer des variables temporelles supplémentaires et des méthodes d'évaluation plus adaptées aux données chronologiques.

## Contribution

Projet réalisé en groupe dans le cadre de la Licence 3.
