# 🧠 Clustering iNaturalist - Hackathon [LEPL1109]

Projet universitaire réalisé dans le cadre du cours **STATISTICS AND DATA SCIENCES** à l'UCLouvain.

## 🎯 Objectif

Développer une méthode de **clustering non supervisé** pour analyser un sous-ensemble du dataset *iNaturalist* (observations biologiques en Belgique), puis affecter une **étiquette taxonomique** à chaque cluster et évaluer la capacité du modèle à **prédire le niveau "order"** d'observations inédites.

## 🗂️ Données

- Observations géolocalisées de plantes et d’animaux issues de *iNaturalist*
- Taxonomie biologique complète (kingdom → species)
- Variables temporelles et spatiales dérivées (saison, moment de la journée, week-end...)

## 🛠️ Méthodologie

- Nettoyage, encodage et enrichissement du dataset
- Réduction de dimension via **PCA**
- Clustering par **K-Means**
- Attribution supervisée des clusters via la taxonomie
- Évaluation par validation croisée sur un sous-ensemble test

## 📊 Résultats

- Meilleure précision (~55%) obtenue pour le niveau **order**
- Visualisations saisonnières et spatiales de la distribution des observations
- Comparaison des performances selon le niveau taxonomique prédit (`phylum`, `class`, `order`, `family`)

## 📎 Technologies utilisées

- Python (Pandas, scikit-learn, matplotlib, seaborn, plotly)
- Jupyter Notebook
- Métrique d’évaluation personnalisée fournie par les enseignants

## 👨‍🏫 Encadrement académique

- Prof. Damien Hainaut  
- Prof. Laurent Jacques  
- UCLouvain – 2023

## 📄 Fichiers

- `hackathon03_clustering.ipynb` – Notebook principal
- `toolbox.py` – Fonctions utilitaires fournies
- `Data/inaturalist_be.csv` – Jeu de données utilisé
