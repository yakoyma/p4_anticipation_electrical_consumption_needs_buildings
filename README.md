# Projet 4 : Anticipez les besoins en consommation électrique de bâtiments

Parcours Data Scientist d'OpenClassrooms en partenariat avec CentraleSupélec.

L'objectif du projet est de prédire les émissions de CO2 et la consommation totale d'énergie de bâtiments non résidentiels de la ville de Seattle. Il s'agit d'un problème de régression. Il faut donc comparer les différents algorithmes de Machine Learning et évaluer leurs performances pour sélectionner le modèle le plus adapté au problème métier.

Le jeu de données est composé de 2 fichiers csv :
- Le jeu de données 2015-building-energy-benchmarking ;
- Le jeu de données 2016-building-energy-benchmarking.

La source des données est la suivante : https://data.seattle.gov/dataset/2016-Building-Energy-Benchmarking/2bpz-gwpy


## Les étapes de l'analyse exploratoire courte :
- L'import des jeux de données 2015 et 2016 ;
- La transformation de features et la création de nouvelles variables pertinentes ;
- Le feature engineering et l'exploration du jeu de données ;
- L'analyse univariée :
  - L'analyse des indicateurs statistiques classiques ;
  - L'analyse des distributions de variables ;
  - Le test d'adéquation des variables à une loi normale (utilisation du package pingouin) ;
  - Le test d'égalité des variances (utilisation du package pingouin). 
- L'analyse multivariée :
  - L'analyse des corrélations entre les variables quantitatives ;
  - L'analyse bivariée entre les variables quantitatives et catégorielles ;
  - L'analyse de la variance par la méthode ANOVA.


## Les étapes des différents tests des modèles de Machine Learning (linéaires, non linéaires et ensemblistes) pour la prédiction d'émissions de CO2 et de la consommation totale d'énergie de bâtiments :
- L'import du jeu de données nettoyé ;
- Feature engineering (application de la transformation logarithmique pour normaliser les variables cibles) ;
- Les différents tests des modèles de régression, l'évaluation des performances des modèles et prédictions (utilisation de la librairie Sklearn) :
  - La réalisation d'un pipeline complet de prédiction ; 
  - La comparaison des modèles avec les hyperparamètres de base par validation croisée ;
  - La comparaison des modèles avec les hyperparamètres optimisés par validation croisée ;
  - La sélection du modèle supervisé adapté au problème métier ;
  - L'interprétabilité globale et locale du modèle ;
  - L'optimisation des hyperparamètres du modèle par validation croisée ;
  - La prédiction des valeurs normalisées des variables cibles par le modèle avec les hyperparamètres optimisés ;
  - La prédiction des valeurs réelles des variables cibles par le modèle avec les hyperparamètres optimisés (en bonus).


