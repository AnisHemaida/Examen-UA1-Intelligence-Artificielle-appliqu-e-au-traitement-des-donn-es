# 💳 Détection de fraude par carte de crédit  
Projet UA3 – Analyse de données & Intelligence Artificielle  

## 🎯 Objectif du projet
L’objectif de ce projet est de développer un modèle de détection de transactions frauduleuses à partir d’un dataset de transactions bancaires.  
Le projet vise à :

- Analyser les données transactionnelles
- Gérer le déséquilibre des classes (fraude vs non-fraude)
- Construire et évaluer des modèles de classification
- Interpréter les résultats obtenus

---

## 📊 Contexte
La fraude par carte de crédit représente un enjeu majeur pour les institutions financières.  
Les transactions frauduleuses sont rares, ce qui crée un fort déséquilibre des classes et rend la détection plus complexe.

---

## 📂 Dataset
- Source : Dataset public (Credit Card Fraud Detection)
- Nombre d’observations : 284 807 transactions
- Variable cible : `Class`
  - 0 → Transaction normale
  - 1 → Transaction frauduleuse

⚠️ Le fichier `creditcard.csv` n’est pas inclus dans ce dépôt (fichier volumineux).  
Téléchargez le dataset depuis la source officielle (Kaggle) et placez-le dans le dossier du projet.

---

## 🔎 Méthodologie

### 1️⃣ Préparation des données
- Vérification des valeurs manquantes
- Analyse statistique descriptive
- Normalisation de la variable `Amount`
- Gestion du déséquilibre des classes

### 2️⃣ Analyse exploratoire (EDA)
- Distribution des classes
- Visualisation des corrélations
- Analyse des variables les plus influentes

### 3️⃣ Modélisation
Plusieurs modèles ont été testés :

- Régression Logistique
- Random Forest
- Autres modèles de classification

### 4️⃣ Évaluation
Les performances ont été mesurées à l’aide de :

- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC

Une attention particulière a été portée au **Recall**, afin de minimiser les faux négatifs (fraudes non détectées).

---

## 📈 Résultats principaux
- Le modèle Random Forest offre une meilleure capacité de détection
- Le déséquilibre des classes impacte fortement les métriques classiques
- L’optimisation du Recall améliore la détection des fraudes

---

## 🛠 Technologies utilisées
- Python
- Pandas
- NumPy
- Matplotlib / Seaborn
- Scikit-learn
- Jupyter Notebook
