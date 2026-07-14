![Python](https://img.shields.io/badge/Python-blue?logo=python) ![Jupyter](https://img.shields.io/badge/Jupyter-orange?logo=jupyter) ![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

# Analyse des ventes d'une boutique de vins

Ce projet présente une analyse de données réalisée à partir de plusieurs fichiers liés à l'activité d'une boutique de vins en ligne.

L'idée était d'explorer les données disponibles, de vérifier leur qualité, puis d'en tirer quelques premiers constats sur les ventes, les stocks et la rentabilité des produits.

## À propos du projet

Le travail s'appuie sur plusieurs sources de données : catalogue produits, informations de stock, ventes et données issues du site e-commerce.

L'objectif n'était pas seulement de produire quelques indicateurs, mais aussi de repartir sur une base propre et cohérente. Une partie importante du projet a donc consisté à repérer les valeurs manquantes, les doublons et certaines incohérences dans les données avant de passer à l'analyse.

## Ce qu'on trouve dans ce repo

- `project_bottleneck.ipynb` : notebook principal avec le nettoyage, les contrôles qualité, la fusion des données et l'analyse.
- éventuellement d'autres fichiers de données ou notebooks complémentaires selon l'organisation du projet.
- `README.md` : présentation du projet.

## Ce qui a été fait

Dans ce notebook, on retrouve notamment :

- un contrôle de la qualité des données ;
- la mise en relation de plusieurs fichiers ;
- une analyse des ventes par produit ;
- un travail autour du chiffre d'affaires ;
- une première lecture des marges ;
- quelques points d'attention sur les stocks.

L'idée était surtout de mieux comprendre l'activité et d'identifier les produits qui ressortent, soit par leurs ventes, soit par leur rentabilité, soit par des écarts entre stock et niveau de vente.

## Outils utilisés

Le projet a été réalisé en Python, principalement avec :

- `pandas`
- `numpy`
- `matplotlib` / `seaborn`
- Jupyter Notebook

## Lancer le projet

1. Cloner le repo :

```bash
git clone https://github.com/cedizen/wine_store_sales.git
cd wine_store_sales
```

2. Créer un environnement virtuel si besoin :

```bash
python -m venv .venv
source .venv/bin/activate
```

Sous Windows :

```bash
.\.venv\Scripts\activate
```

3. Installer les dépendances si un fichier `requirements.txt` est ajouté :

```bash
pip install -r requirements.txt
```

4. Lancer Jupyter Notebook :

```bash
jupyter notebook
```

5. Ouvrir `project_bottleneck.ipynb` et exécuter les cellules dans l'ordre.

## Pourquoi ce projet

Ce projet correspond à une première phase d'analyse : comprendre les données, les fiabiliser et commencer à dégager quelques enseignements utiles.

C'est un travail assez proche de ce qu'on peut faire au début d'une mission data : avant de vouloir aller vers du prédictif ou du dashboard, il faut déjà savoir si les données sont propres, reliables et exploitables.

## Pistes pour aller plus loin

Quelques prolongements possibles :

- ajouter plus de visualisations ;
- construire un petit dashboard ;
- approfondir l'analyse des marges ;
- travailler sur l'optimisation des stocks ;
- tester une approche de prévision des ventes.

## Auteur

Projet réalisé par Cédric Berthezene.

GitHub : [cedizen](https://github.com/cedizen)
