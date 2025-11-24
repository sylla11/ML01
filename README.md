# 🏠 Prédiction du Prix des Maisons - Ames Housing Dataset


Projet complet de Machine Learning pour prédire le prix des maisons en utilisant le célèbre dataset Ames Housing. Ce projet démontre un pipeline complet de Data Science, de l'exploration des données à la modélisation prédictive.

## 📊 Aperçu du Projet

Ce projet a été réalisé dans le cadre du Master 2 Data Science et Machine Learning à l'INPHB. Il met en œuvre un processus complet d'analyse de données et de modélisation prédictive sur le dataset Ames Housing, contenant des informations sur ~2930 ventes de propriétés résidentielles.

### 🎯 Objectifs

- Analyser en profondeur les facteurs qui influencent le prix des propriétés
- Nettoyer et préparer les données pour la modélisation
- Construire un modèle prédictif robuste et interprétable
- Évaluer les performances et identifier les variables clés
- Fournir des recommandations actionnables

## 📈 Résultats Clés

| Métrique | Valeur | Interprétation |
|----------|--------|----------------|
| **R² Score** | 82.60% | Excellent niveau de prédiction |
| **RMSE** | $37,349 | Erreur quadratique moyenne |
| **MAE** | $17,501 | Erreur typique (~10% du prix moyen) |
| **Erreur moyenne** | -0.71% | Pas de biais systématique |

✅ **Le modèle explique 82.60% de la variance des prix !**

## 🗂️ Structure du Projet

```
ames-housing-prediction/
│
├── notebook_final_enrichi.ipynb    # Notebook principal avec analyses complètes
├── AmesHousing.csv                 # Dataset (à télécharger)
├── README.md                       # Ce fichier
├── requirements.txt                # Dépendances Python                       # Licence MIT
└── .gitignore                      # Fichiers à ignorer
```

## 🛠️ Technologies Utilisées

- **Python 3.8+**
- **pandas** - Manipulation de données
- **numpy** - Calculs numériques
- **scikit-learn** - Machine Learning
- **matplotlib** - Visualisations
- **seaborn** - Visualisations statistiques
- **scipy** - Analyses statistiques

## 📋 Table des Matières du Notebook

### Partie I : Préparation et Exploration
1. **Importations et Configuration**
2. **Chargement et Exploration Initiale**
3. **Nettoyage et Traitement des Valeurs Manquantes**

### Partie II : Analyses Statistiques
4. **Analyse Univariée**
5. **Analyse Bivariée** (Variables numériques et catégorielles)
6. **Analyse Multivariée** (Corrélations et multicolinéarité)

### Partie III : Modélisation
7. **Feature Engineering et Préparation**
   - Transformation logarithmique
   - Encodage des variables catégorielles
   - Division Train/Test
   - Standardisation
8. **Modélisation et Évaluation** (Régression Linéaire)
9. **Interprétation Approfondie des Résultats**

## 🚀 Installation et Utilisation

### Prérequis

- Python 3.8 ou supérieur
- Jupyter Notebook ou JupyterLab

### Installation

1. **Cloner le repository**
```bash
git clone https://github.com/VOTRE_USERNAME/ames-housing-prediction.git
cd ames-housing-prediction
```

2. **Créer un environnement virtuel** (recommandé)
```bash
python -m venv venv
source venv/bin/activate  # Sur Windows: venv\Scripts\activate
```

3. **Installer les dépendances**
```bash
pip install -r requirements.txt
```

4. **Télécharger le dataset**

Téléchargez le fichier `AmesHousing.csv` depuis [Kaggle](https://www.kaggle.com/datasets/prevek18/ames-housing-dataset) ou utilisez le lien direct du cours et placez-le dans le dossier racine.

5. **Lancer Jupyter Notebook**
```bash
jupyter notebook notebook_final_enrichi.ipynb
```

## 📊 Méthodologie

### 1. Nettoyage des Données

- **Traitement des valeurs manquantes** : Imputation par médiane (numériques) et mode (catégorielles)
- **Suppression de colonnes** : >50% de valeurs manquantes
- **Gestion des outliers** : Conservation avec transformation log

### 2. Feature Engineering

- **Transformation logarithmique** : Normalisation de la variable cible
  - Réduction de skewness de 1.88 → 0.12
  - Amélioration de R² : +5-10 points
- **Encodage catégoriel** : Label Encoding pour ~30 variables
- **Standardisation** : Z-score (μ=0, σ=1) pour toutes les features

### 3. Modélisation

- **Algorithme** : Régression Linéaire Multiple (OLS)
- **Division** : 80% train / 20% test
- **Validation** : Évitement rigoureux du data leakage

## 🔑 Variables les Plus Importantes

| Rang | Variable | Coefficient | Impact |
|------|----------|-------------|--------|
| 1 | BsmtFin SF 1 | +0.419 | Surface sous-sol fini |
| 2 | Bsmt Unf SF | +0.393 | Surface sous-sol non fini |
| 3 | Overall Qual | +0.109 | Qualité générale |
| 4 | Gr Liv Area | +0.065 | Surface habitable |
| 5 | Garage Cars | +0.041 | Capacité garage |

## 📈 Visualisations Clés

Le notebook contient plus de 15 visualisations professionnelles :
- Distributions avant/après transformation
- Matrices de corrélation
- Scatter plots des variables principales
- Analyse des résidus
- Comparaisons train/test

## 💡 Insights et Recommandations

### Points Forts du Modèle

✅ **Performance excellente** : R² = 82.60%  
✅ **Simplicité** : Modèle linéaire interprétable  
✅ **Robustesse** : Pas de biais systématique  
✅ **Praticité** : Rapide à entraîner et déployer

### Axes d'Amélioration

🚀 **Quick Wins** (+2-5% R²) :
- Feature engineering avancé (interactions, ratios)
- Traitement spécifique des outliers
- Régularisation (Ridge/Lasso)

🚀 **Améliorations Avancées** (+5-10% R²) :
- Random Forest / XGBoost
- Ensemble methods
- Cross-validation rigoureuse

## 🎓 Compétences Démontrées

- ✅ **Data Cleaning** : Gestion des valeurs manquantes, outliers
- ✅ **EDA** : Analyses univariée, bivariée, multivariée
- ✅ **Feature Engineering** : Transformations, encodage, standardisation
- ✅ **Modeling** : Pipeline ML complet, prévention du data leakage
- ✅ **Evaluation** : Métriques multiples, validation rigoureuse
- ✅ **Communication** : Documentation exhaustive, visualisations professionnelles

## 📱 Applications Pratiques

1. **Estimation pour vendeurs** : Aide à la fixation du prix
2. **Évaluation pour acheteurs** : Détection des bonnes affaires
3. **Analyse d'investissement** : Calcul de ROI après rénovation
4. **Études de marché** : Identification des drivers de valeur

## 👤 Auteur

**SYLLA Oumarou**  
Master 2 - Data Science et Machine Learning  
INPHB (Institut National Polytechnique Houphouët-Boigny)  
Côte d'Ivoire