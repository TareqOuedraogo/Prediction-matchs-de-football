# Prediction-matchs-de-football
Machine learning models to predict football match outcomes using historical data

Contexte:
Dans ce projet, vous devez créer des modèles d’IA dans le but de prédire le résultat de matchs de football (soccer) de deux équipes. Ce projet comporte deux facettes : 1. la soumission d’un Jupyter notebook que vous remettrez sur eCité dans lequel vous fournirez votre analyse des données ainsi que votre code et 2. une compétion Kaggle, dans laquelle vous tenterez de battre les scores de vos camarades de classe.

Instructions
football.csv - Le fichier a utiliser pour entraîner vos modèles

competition.csv - Le fichier de compétition que vous devez prédire avec votre modèle entraîné.

exemple_soumission.csv - Un exemple du format de fichier que vous devez soumettre sur Kaggle

Confert document d'instructions pour les instructions détaillées

Colonnes
Note : X dans le nom de la caractéristique est soit home ou away, indiquant si la caractéristique est pour l’équipe à domicile ou l’équipe extérieure.

• 'id': Identifiant unique.

• 'date': La date où le match a eu lieu.

• 'X_team': Le nom de l’équipe.

• 'rank_change_X': Le changement au classement FIFA pour l'équipe entre la période de classement actuelle et la période de classement précédente. Les valeurs négatives indiquent une baisse du classement, tandis que les valeurs positives indiquent une amélioration.

• 'X_goals_mean': Nombre moyen de buts marqués par l'équipe dans tous les matchs précédents.

• 'X_goals_mean_l5': Nombre moyen de buts marqués par l'équipe dans les 5 derniers matchs.

• 'X_goals_suf_mean': Moyenne des buts subis par l'équipe dans tous les matchs précédents.

• 'X_goals_suf_mean_l5': Moyenne des buts subis par l'équipe dans les 5 derniers matchs.

• 'X_rank_mean': Classement FIFA moyen de l'équipe lors de tous les matchs précédents.

• 'X_rank_mean_l5': Classement FIFA moyen de l'équipe lors des 5 derniers matchs.

• 'X_points_mean': Moyenne des points obtenus par l'équipe à domicile/à l'extérieur (victoire=3, match nul=1, défaite=0) dans tous les matchs prédécents.

• 'X_points_mean_l5': Moyenne des points obtenus par l'équipe à domicile/à l'extérieur (victoire=3, match nul=1, défaite=0) dans les 5 derniers matchs. •

'match_type: Si le match est un tournoi amical (friendly) ou un match de compétition (competition). •

'target': Le résultat du match. 1 pour une victoire, 0 pour une défaite ou un match nul.

Objectifs1. Analyse exploratoire des données
Code et explications (commentaires) pour :

Visualisations : Histogrammes, diagrammes en boîte, matrices de corrélation et autres graphiques pour mettre en évidence les tendances, les déséquilibres ou les valeurs aberrantes.

Résumé statistique : moyenne, variance, asymétrie, valeurs manquantes et répartition par classe (le cas échéant).

Identification des problèmes potentiels (valeurs manquantes, valeurs aberrantes, données déséquilibrées)

Prétraitement Code et explications (commentaires) pour votre prétraitement, incluant, si nécessaire :
Valeurs manquantes (imputation, suppression, etc.)

Valeurs aberrantes (méthode de détection + stratégie utilisée)

Données catégorielles (OHE, ordinal, etc.)

Séparation des données : Répartition entraînement/test ou de la validation croisée choisie

Mise à l'échelle des caractéristiques (normalisation/standardisation)

Éviter les fuites de données

Développement des modèles et expérimentation Minimum de 4 modèles (1 de chaque catégorie) :
Modèle linéaire/régularisé (par exemple, régression Ridge/Lasso)

Modèle à base d'arbres

SVM

KNN

Réglage des hyperparamètres : Changer les hyperparamètres d'un minimum de 2 modèles avec justification puis comparer les performances

Documentation claire des paramètres des modèles testés

Évaluation finale et comparaison des modèles Comparaison des modèles avec l'usage des mesures de performance appropriées (par exemple, précision, score F1, ROC-AUC, MSE, MAE, …)
Comparaison visuelle (par exemple, Courbes ROC, matrices de confusion ou courbes d'apprentissage, …)

Discussion finale Discussion des points clés, par exemple :
Discussion et conclusions tirées de l'exploration des données

Sommaire des prétraitements testés/effectués, qu'est-ce qui a fonctionné/n'a pas fonctionné ? Pourquoi vous avez fait chaque étape de prétraitement et pourquoi avoir choisi celle-ci ?

Détails des modèles testés, qu'est-ce qui a fonctionné/n'a pas fonctionné ? Pourquoi selon-vous ?

Discussion des performances obtenues, est-ce que les performances obtenues ont été satisfaisantes ? Est-ce que vous avez remarqué des différences entre les différentes métriques ? Pourquoi selon-vous ?

Discussion sur le meilleur et le pire modèle obtenu, pourquoi selon-vous ?

Conclusions finales, quelles sont les limitations de votre modèle ? Qu'est-ce qu'on pourrait faire pour améliorer les performances comme travail futur ?
