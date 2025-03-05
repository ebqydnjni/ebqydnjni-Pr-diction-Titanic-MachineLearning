# Prediction-Titanic-MachineLearning
# 🚢 **Projet d'Analyse des Données : Titanic**

##  Professeur :
- **Docteur YOSRA HAJJAJI** 🌟

---

### 🎓 **Matière** : Introduction à l'Intelligence Artificielle

### Date : *04/03/2025* ✍️
👨‍💻 Étudiant : Aldiouma Mbaye
---

## 📌 **Objectif du Projet**
L'objectif de ce projet est d'analyser les données des passagers du Titanic afin de prédire leur probabilité de survie en fonction de différentes caractéristiques telles que l'âge, le sexe, la classe sociale, etc. Ce projet met en œuvre des techniques de **prétraitement des données**, d'**exploration**, et de **modélisation** via des algorithmes de Machine Learning.

---

## 📂 **Description des Données**
Le dataset est composé de plusieurs fichiers :

- **train.csv** : Ensemble d'entraînement contenant les passagers avec leur statut de survie.
- **test.csv** : Ensemble de test utilisé pour l'évaluation du modèle.
- **gender_submission.csv** : Exemple de prédictions attendues.
- **Titanic_Dataset.csv** : Une version alternative combinant les données.

### 🏷️ **Attributs Principaux**
- `PassengerId` : Identifiant unique du passager
- `Survived` : Statut de survie (1 = Oui, 0 = Non)
- `Pclass` : Classe du passager (1ère, 2ème, 3ème)
- `Name` : Nom du passager
- `Sex` : Sexe du passager
- `Age` : Âge du passager
- `SibSp` : Nombre de frères/sœurs/conjoints à bord
- `Parch` : Nombre de parents/enfants à bord
- `Ticket` : Numéro du billet
- `Fare` : Tarif du billet
- `Cabin` : Numéro de cabine
- `Embarked` : Port d'embarquement (C = Cherbourg, Q = Queenstown, S = Southampton)

---

## 🛠️ **Étape 1 : Prétraitement des Données**
Avant d'entraîner un modèle, nous devons nettoyer et transformer les données :

1. **Gestion des valeurs manquantes**
   - Imputation des valeurs manquantes (`Age`, `Embarked`, `Cabin`)
   - Suppression ou transformation de certaines variables

2. **Encodage des variables catégorielles**
   - Mapping `Sex` (`male → 0`, `female → 1`)
   - Encodage One-Hot de `Embarked`

3. **Mise à l’échelle des variables**
   - Standardisation de `Age` et `Fare`

4. **Gestion des outliers**
   - Transformation logarithmique de `Fare`

---

## 🤖 **Étape 2 : Modélisation et Prédiction**
Après le prétraitement, nous allons entraîner plusieurs modèles de classification pour prédire la survie des passagers :

- **Régression Logistique**
- **K-Nearest Neighbors (KNN)**
- **Random Forest**
- **Gradient Boosting**

Nous comparerons les performances de chaque modèle à l’aide des **métriques d’évaluation** comme l’**exactitude (accuracy)**, la **matrice de confusion**, et l’**AUC-ROC**.

---

## 📊 **Étape 3 : Analyse et Visualisation des Résultats**
Nous utiliserons des bibliothèques comme **Matplotlib**, **Seaborn** et **Plotly** pour explorer et visualiser les résultats.

### 🔍 **Quelques analyses prévues :**
- Taux de survie par classe et sexe
- Influence de l’âge sur la survie
- Corrélations entre les variables

---

## 🎯 **Conclusion et Perspectives**
Nous conclurons en analysant les performances du modèle final et en suggérant des améliorations possibles, telles que l'utilisation de modèles plus avancés (**Deep Learning**, **Feature Engineering**, etc.).
