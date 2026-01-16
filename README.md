# 💡 Impact des investissements marketing sur les ventes
**Prédire les ventes à partir des investissements publicitaires**

---

## 🧠 Contexte

Une entreprise souhaite mieux comprendre l’impact de ses dépenses publicitaires sur ses ventes.  
Elle dispose d’un jeu de données comprenant les montants investis dans trois canaux de communication :

- 📺 TV  
- 📻 Radio  
- 📰 Presse écrite (Newspaper)  

ainsi que les ventes correspondantes.

L’objectif est d’exploiter ces données afin de construire un **modèle de prédiction fiable** permettant d’estimer les ventes en fonction des budgets publicitaires.

---

## 🎯 Objectif du projet

- Analyser l’impact des investissements publicitaires sur les ventes
- Identifier les canaux les plus influents
- Construire un modèle de **régression linéaire** pour prédire les ventes
- Mettre en place un pipeline complet :
  - exploration
  - nettoyage
  - modélisation
  - évaluation
  - utilisation du modèle

---

## ❓ Questions clés

- Quels canaux publicitaires influencent le plus les ventes ?
- Existe-t-il une relation linéaire entre les investissements publicitaires et les ventes ?
- Peut-on prédire efficacement les ventes à partir des budgets publicitaires ?

---

## 📁 Description du dataset

Le dataset contient 200 observations et 4 variables :

```bash

| Variable    | Description                                  |
|------------|----------------------------------------------|
| TV         | Budget investi en publicité TV               |
| Radio      | Budget investi en publicité Radio            |
| Newspaper  | Budget investi en publicité Presse écrite    |
| Sales      | Ventes générées                              |

Le dataset brut est disponible dans :  
`data/raw/advertising.csv`

```

---

## 🔍 Méthodologie

### 1️⃣ Exploration des données (EDA)

- Analyse statistique descriptive
- Visualisation des distributions
- Analyse des corrélations entre variables
- Identification des tendances et relations

### 2️⃣ Préparation des données

- Vérification des valeurs manquantes
- Détection des valeurs aberrantes (outliers)
- Décision argumentée de conservation des outliers
- Séparation des données en jeux d’entraînement et de test

### 3️⃣ Modélisation

- Implémentation d’un modèle de **régression linéaire multivariée**
- Entraînement sur le jeu d’apprentissage
- Interprétation des coefficients

### 4️⃣ Évaluation du modèle

- Évaluation sur le jeu de test
- Métriques utilisées :
  - RMSE
  - R²
- Visualisation des prédictions vs valeurs réelles

### 5️⃣ Utilisation du modèle

- Sauvegarde du modèle entraîné (`.pkl`)
- Chargement du modèle
- Prédiction des ventes à partir de nouveaux scénarios d’investissement

---

## 📊 Résultats principaux

- 📺 **La TV est le canal le plus influent** sur les ventes
- 📻 La Radio a un impact positif mais secondaire
- 📰 La presse écrite a un impact limité
- Le modèle explique environ **90 % de la variance des ventes (R² ≈ 0.9)**

---

## 🧱 Structure du projet

```bash

Marketing-Spend-Analysis-and-Sales-Forecasting/
│
├── data/
│   ├── raw/
│   │   └── advertising.csv
│   └── processed/
│       └── advertising_cleaned.csv
│
├── notebooks/
│   ├── 01_Data_Cleaning.ipynb
│   ├── 02_EDA_Statistics.ipynb
│   └── 03_Linear_Regression_Modeling.ipynb
│
├── models/
│   └── linear_regression_sales.pkl
│
└── README.md
```

---

## 🛠️ Technologies utilisées

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Joblib

---

## 🚀 Conclusion

Ce projet illustre un **pipeline complet d’analyse de données et de modélisation prédictive**, depuis l’exploration des données jusqu’à l’utilisation concrète d’un modèle de machine learning.  
Il met en évidence l’importance de la TV dans la génération des ventes et démontre l’efficacité d’une régression linéaire pour ce type de problématique métier.
