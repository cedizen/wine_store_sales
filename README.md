![Python](https://img.shields.io/badge/Python-blue?logo=python) ![Jupyter](https://img.shields.io/badge/Jupyter-orange?logo=jupyter) ![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

# Projet : analyse des données de stock et de ventes d'un site de vente en ligne de vin

## Présentation du projet

Ce projet a pour objectif d’analyser les données de stock, de ventes et de prix d’un site de vente en ligne de vins, afin d’identifier les produits phares, les surstocks, les marges optimales et les tendances de prix. L’analyse repose sur la fusion de données issues d’un ERP, du site web et d’un fichier de liaison entre les deux systèmes.

## Objectifs du Projet

*   **Exploration des données** : nettoyer et comprendre la structure des données issues de l'ERP, du site web et du fichier de liaison.  
*   **Analyse des prix** : identifier les prix aberrants et les justifier.  
*   **Analyse des ventes** : calculer le Chiffre d’Affaires (CA), analyser les quantités vendues et identifier les produits phares et ceux moins performants.  
*   **Analyse des stocks** : évaluer la rotation des stocks, valoriser le stock total et détecter les surstocks potentiels.  
*   **Analyse de la marge** : calculer le taux de marge et la marge brute par produit et par catégorie.  
*   **Corrélations** : étudier les relations entre les variables clés (prix, stock, ventes) pour identifier des tendances.

## Données utilisées

Trois fichiers Excel ont été utilisés et fusionnés pour cette analyse :

*   'erp.xlsx' : informations produit du système ERP (ID, prix, quantité en stock, prix d’achat).  
*   'web.xlsx' : données produits du site web (référence SKU, ventes totales, type de produit).  
*   'liaison.xlsx' : fichier de correspondance entre 'product_id' (ERP) et 'id_web' (site web).

## Résultats clés et insights

*   **Nettoyage des données** : correction des prix négatifs, gestion des incohérences de statut de stock et traitement des SKU mal formatés ou manquants.  
*   **Identification des outliers de prix** : certains produits à prix très élevés ont été repérés, mais ils correspondent à une gamme de vins haut de gamme légitime, représentant environ 4,62 % du catalogue.  
*   **Chiffre d’Affaires (CA)** : le CA global du site est de 153 365,7 € TTC. Le principe de Pareto indique que près de 58,85 % des articles génèrent 80 % du CA.  
*   **Rotation des stocks** : certains produits, notamment dans la catégorie “Champagne”, présentent une rotation de stock très faible, suggérant des surstocks possibles.  
*   **Taux de marge** : après correction d’une erreur de saisie importante (-634,99 % corrigée), le taux de marge s’étend désormais de 22,78 % à 47,76 %.  
*   **Corrélations** :  
    *   forte corrélation (0,98) entre le prix d’achat ('purchase_price') et le prix de vente ('prix_HT'), ce qui est cohérent avec la logique de rentabilité ;  
    *   corrélations faibles mais indicatives entre stock, ventes et prix, suggérant que des stocks plus élevés et des prix plus bas tendent à être associés à des volumes de ventes légèrement supérieurs.
