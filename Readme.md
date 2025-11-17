
**Analyse de la consommation énergétique dans l'industrie**

**Table des matières**
Aperçu
Objectifs
Jeu de données
Méthodologie
Étapes du Notebook
Modèles utilisés
Résultats
Structure du projet
Installation
Utilisation
Améliorations futures
Auteur
Licence

---

**Aperçu**
Ce projet analyse un jeu de données industriel afin d’étudier la consommation énergétique dans une usine sidérurgique.
L’objectif est de comprendre les tendances, d’explorer les données et de construire un modèle prédictif performant.

---

**Objectifs**

* Analyser les tendances temporelles
* Étudier les relations entre variables
* Nettoyer et préparer les données
* Réaliser une EDA complète
* Construire des modèles de régression
* Comparer baseline, LightGBM et Prophet

---

**Jeu de données**
Le dataset contient :

* Une variable temporelle (Date_Time)
* Plusieurs variables industrielles
* Une variable cible : consommation énergétique

Format : CSV
Source : Notebook Kaggle

---

**Méthodologie**
La démarche suit les étapes suivantes :

1. Importation des bibliothèques
2. Chargement des données
3. Inspection initiale
4. Nettoyage
5. Feature Engineering
6. Visualisations
7. Split train/test
8. Modélisation (LightGBM + Prophet)
9. Évaluation

---

**Étapes du Notebook**

**1. Import des bibliothèques et lecture des données**
Chargement du dataset et première exploration.

**2. Inspection initiale**

* Dimensions
* Types
* Valeurs manquantes
* Statistiques de base

**3. Nettoyage**

* Conversion de Date_Time
* Gestion des valeurs manquantes
* Conversion numérique

**4. Feature Engineering**
Extraction de : année, mois, jour, heure, weekday, etc.

**5. Visualisations**

* Analyse temporelle
* Distributions
* Heatmap des corrélations

**6. Split Train/Test**
Séparation des données en ensembles d’entraînement et de test.

**7. Modélisation**

* Baseline simple
* LightGBM comme modèle principal
* Prophet pour modélisation temporelle

**8. Évaluation**
Metrics typiques : RMSE, MAE, R².

---

**Modèles utilisés**

**Baseline**
Modèle simple utilisé comme référence.

**LightGBM**
Modèle performant pour données tabulaires.

**Prophet**
Modèle de prévision temporelle développé par Meta (Facebook).
Il permet :

La décomposition tendance + saisonnalité

La prise en compte des variations journalières et hebdomadaires

La prédiction future de la consommation énergétique
Il est particulièrement adapté aux séries temporelles industrielles.

---

**Résultats**
Les résultats incluent :

Score RMSE

Score MAE

Score R²

Importance des features (LightGBM)

Courbes de tendance et saisonnalité (Prophet)...

---

**Structure du projet**

```
projet-consommation-energetique/
│
├── analyse_energie.ipynb
├── data/
├── README.md
└── requirements.txt
```

---

**Installation**

```
git clone https://github.com/Ghizlane1998/prevision-energie-siderurgie.gitc:\Users\Hp\Downloads\archive (2)\Steel_industry.csv
cd TON-REPO
pip install -r requirements.txt
```

---

**Utilisation**

```
jupyter analyse-de-la-consommation-nerg-tique.ipynb
```

Ou ouvrir le notebook dans VS Code.

---

**Améliorations futures**

* Optimisation avancée
* Tests avec XGBoost et CatBoost
* Détection d’anomalies
* Dashboard Streamlit
* Intégration MLOps

---

# Auteur

**Ghizlane Lamzouri**
Ingénieure en Intelligence Artificielle & Data Scientist
EILCO – École d'Ingénieurs du Littoral Côte d'Opale

---

**Licence**
Licence MIT.
