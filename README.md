# **Prêt à dépenser - Scoring Crédit**

Ce projet fait partie de la mission de développement d'un outil de scoring pour la société **Prêt à dépenser**, visant à prédire si un client remboursera ou non un crédit à la consommation. 

---

## **Objectifs du projet**
L'objectif principal est de développer un modèle de classification capable de :
- Prédire la probabilité qu'un client rembourse un crédit.
- Classer les demandes en **crédit accordé** ou **crédit refusé**.
- Fournir une interprétabilité globale et locale pour aider les chargés de relation client à comprendre les décisions du modèle.

---

## **Contraintes spécifiques**
1. **Gestion du déséquilibre des classes** :
   - Le déséquilibre entre les bons et mauvais clients doit être pris en compte dans le modèle.
2. **Optimisation des coûts métier** :
   - Un faux négatif (FN) a un coût 10 fois supérieur à un faux positif (FP).
   - Définir un seuil optimal pour minimiser le coût métier.
3. **Interprétabilité** :
   - L'importance des variables doit être analysée globalement et localement pour un client donné.

---

## **Structure des fichiers**
Le projet est organisé comme suit :
- **Notebooks principaux** :
  - `Lecerf_Yann_1_notebook_analyse_exploratoire_feature_engineering_092024.ipynb` : Contient les étapes de l’analyse exploratoire des données et le feature engineering.
  - `Lecerf_Yann_2_notebook_modelisation.ipynb` : Contient les étapes de modélisation, d’évaluation et d’optimisation des modèles.
- **Présentation** :
  - `0-P4_presentation.pdf` : Une présentation synthétique expliquant les étapes clés du projet et les résultats obtenus.

---

## **Installation**

### 1. Cloner le projet
```bash
git clone <votre_repo_git>
cd <votre_dossier_de_projet>
```

### 2. Créer et activer un environnement virtuel
#### Linux ou macOS :
```bash
python3 -m venv env
source env/bin/activate
```
#### Windows :
```bash
python -m venv env
env\Scripts\activate
```

### 3. Installer les dépendances
```bash
pip install -r requirements.txt
```

### 4. Préparer le jeu de données
- Créez un dossier `data` à la racine du projet.
- Téléchargez le jeu de données à partir de ce [lien](https://s3-eu-west-1.amazonaws.com/static.oc-static.com/prod/courses/files/Parcours_data_scientist/Projet+-+Impl%C3%A9menter+un+mod%C3%A8le+de+scoring/Projet+Mise+en+prod+-+home-credit-default-risk.zip) et placez-le dans le dossier `data` et dézipper-le.

---

## **Utilisation**

1. **Analyse exploratoire et feature engineering** :
   - Lancez le notebook `Lecerf_Yann_1_notebook_analyse_exploratoire_feature_engineering_092024.ipynb` pour nettoyer les données, gérer les valeurs manquantes et construire de nouvelles variables prédictives.

2. **Modélisation et optimisation** :
   - Lancez le notebook `Lecerf_Yann_2_notebook_modelisation.ipynb` pour entraîner et évaluer plusieurs modèles de classification, optimiser les hyperparamètres, et calculer des métriques d’évaluation.

3. **Présentation des résultats** :
   - Consultez le fichier `Lecerf_Yann_3_presentation_092024.pdf` pour une synthèse des étapes du projet et des résultats obtenus.

---

## **Technologies utilisées**

![Python](https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=blue)
![Pandas](https://img.shields.io/badge/Pandas-2C2D72?style=for-the-badge&logo=pandas&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![LightGBM](https://img.shields.io/badge/LightGBM-017724?style=for-the-badge&logo=lightgbm&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-FF6600?style=for-the-badge&logo=xgboost&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-007ACC?style=for-the-badge&logo=seaborn&logoColor=white)

---

## **Auteurs**

- [Yann Lecerf](https://github.com/Belin27000)
