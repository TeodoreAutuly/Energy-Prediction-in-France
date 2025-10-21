# Prévision de la Consommation d'Énergie Électrique

## 📋 À propos du projet

Ce projet est un **Travail d'Initiative Personnelle Encadré (TIPE)** réalisé en classe préparatoire par **Téodore Autuly** et **Eloi Kling**.

### Titre complet
**Prévisions de la consommation d'énergie électrique à l'aide de méthodes d'apprentissage**

---

## 🎯 Problématique

**Quelles sont les méthodes d'apprentissage les plus efficaces pour prévoir la consommation d'énergie électrique ?**

### Contexte et motivation

De nos jours, toute énergie électrique produite en excès encourt des pertes importantes. Le stockage de l'électricité nécessite de convertir le courant électrique en une autre forme d'énergie conservable, ce qui engendre :
- Des coûts financiers élevés
- Des pertes énergétiques lors des conversions
- Des problématiques environnementales (bétonnage, barrages hydrauliques, etc.)

Notre objectif est donc de mettre au point des modèles prédictifs destinés à **anticiper la consommation électrique** afin que les producteurs d'électricité puissent ajuster la production à la demande prévue et limiter les pertes.

Les modèles prédictifs développés sont particulièrement efficaces pour prédire la consommation électrique des villes qui suivent des comportements tendanciels et normalisés par la multitude de consommateurs. De plus, ces prévisions favorisent une production d'électricité à proximité des villes, réduisant ainsi les pertes dues au transport de l'énergie.

---

## 🔬 Positionnements thématiques

**Domaines :** INFORMATIQUE (Informatique pratique), INFORMATIQUE (Informatique théorique)

### Mots-clés

| Français | Anglais |
|----------|---------|
| Optimisation | Optimization |
| Apprentissage automatique | Machine learning |
| Renforcement de gradient | Gradient boosting (XGBoost) |
| Base de données | Database |
| Bibliothèque Python Pandas | Python Library Pandas |

---

## 🎓 Objectifs du projet

### Objectifs de Téodore Autuly
- Utiliser et mettre en forme une base de données adaptée au problème
- Réaliser des modèles naïfs de machine learning (statistique et linéaire)
- Confronter les prédictions des modèles entre eux
- Comparer les méthodes entre elles
- Étudier les aspects théoriques du gradient boosting
- Utiliser une autre base de données et réaliser un modèle de machine learning en prenant en compte de nouveaux paramètres

### Objectifs d'Eloi Kling
- Utiliser et mettre en forme une base de données adaptée au problème
- Réaliser des modèles naïfs de machine learning (statistique et polynomial)
- Confronter les prédictions des modèles entre eux
- Réaliser un modèle plus fin de machine learning utilisant le renforcement de gradient
- Comparer les méthodes entre elles
- Étudier l'importance des nouveaux paramètres pris en compte en faisant varier leur utilisation

---

## 📊 Méthodologie et modèles développés

### Approche générale

L'apprentissage automatique (machine learning) permet de prédire un comportement futur à partir d'un comportement passé connu, dont les informations sont répertoriées dans une base de données. Les relevés de consommation énergétique sont précis et accessibles en grande quantité grâce aux nouvelles technologies de compteurs électriques automatiques.

### Types de modèles implémentés

Le projet explore plusieurs approches de régression pour la prédiction de consommation électrique :

1. **Modèles statistiques** (`modele_statistique.ipynb`)
   - Prédictions basées sur les moyennes des consommations des années précédentes
   - Regroupements des données par jours, semaines, mois et années
   - Analyse des tendances saisonnières

2. **Modèles de régression linéaire et polynomiale** (`modele_ml_regression.ipynb`)
   - Régression linéaire avec sklearn
   - Régression polynomiale de degré 5
   - Prise en compte du jour de la semaine et du jour de l'année

3. **Modèles de gradient boosting - XGBoost** (`modele_ml_xgb.ipynb`)
   - Utilisation de XGBoost, le modèle de renforcement de gradient le plus performant
   - Méthode d'apprentissage d'ensemble qui construit successivement de nouvelles feuilles à un arbre de décision
   - Correction itérative des données les moins bien prédites

4. **Modèles avec paramètres additionnels** (`modele_ml_xgb_temp.ipynb`)
   - Intégration de paramètres météorologiques (température)
   - Prise en compte de facteurs temporels, saisonniers et environnementaux
   - Amélioration de la précision des prédictions

### Métriques d'évaluation

Les modèles sont évalués à l'aide de métriques standards :
- **MSE** (Mean Squared Error) - Erreur quadratique moyenne
- **MAE** (Mean Absolute Error) - Erreur absolue moyenne

---

## 📁 Structure du projet

```
Energy-Prediction-France/
│
├── code/                              # Code principal du projet
│   ├── AEP_hourly.csv                # Dataset principal (consommation horaire)
│   ├── DAYTON_hourly.csv             # Dataset secondaire
│   ├── OHDAYTON.csv                  # Dataset avec température
│   ├── dataset_info.ipynb            # Analyse d'informations du dataset
│   ├── dataset_analyse.ipynb         # Analyse exploratoire des données
│   ├── modele_statistique.ipynb      # Modèles statistiques (moyennes)
│   ├── modele_ml_regression.ipynb    # Régressions linéaire et polynomiale
│   ├── modele_ml_xgb.ipynb           # Modèle XGBoost principal
│   ├── modele_ml_xgb_temp.ipynb      # XGBoost avec température
│   └── modele_temp_test_xgb.ipynb    # Tests du modèle avec température
│
├── dataset/                           # Datasets supplémentaires
│   ├── electric_consumption_till_25jun.csv
│   ├── powerconsumption.csv
│   └── temperature.csv
│
├── code_test/                         # Code de test
│   ├── AEP_hourly_test.csv
│   └── test_analyse.ipynb
│
├── to_print/                          # Versions finales pour impression
│   ├── modele_statistique_p.ipynb
│   ├── modele_ml_regression_p.ipynb
│   └── modele_ml_xgb_p.ipynb
│
├── presentation/                      # Documents de présentation
│   ├── presentation.md
│   └── doc.txt
│
├── sources/                           # Références bibliographiques
│
└── MCOT_V3.md                        # Documentation MCOT complète
```

---

## 🔧 Technologies utilisées

### Langages
- **Python** (langage principal)

### Bibliothèques principales
- **Pandas** - Manipulation et analyse de données
- **NumPy** - Calcul numérique
- **Matplotlib / Seaborn** - Visualisation de données
- **scikit-learn** - Modèles de machine learning (régression, métriques)
- **XGBoost** - Algorithme de gradient boosting optimisé

---

## 📚 Bibliographie

[1] EDF. (2021, 14 décembre). *Tout savoir sur le stockage de l'électricité*. https://particulier.edf.fr/fr/accueil/guide-energie/electricite/stockage-energie-electricite.html

[2] Pierre-Thomas Demars, Vincent Imard, Benoît Delinchant. *Machine learning appliqué au domaine de l'énergie — CultureSciences-Physique*. https://culturesciencesphysique.ens-lyon.fr/ressource/IA-energie-Delinchant.xml

[3] Moogsoft. (2019, 16 octobre), Robert Harper. *Understanding the Machine Learning in AIOps*. https://www.moogsoft.com/resources/aiops/white-paper/understanding-machine-learning

[4] Formations Data & Tech - Blent.ai. (2022, 4 Février), Nada Belaidi. *XGBoost : Tout savoir sur le Boosting*. https://blent.ai/xgboost-tout-comprendre/

[5] Barra, V., Miclet, L. & Cornuéjols, A. (2021). *Apprentissage artificiel - 4e édition : Concepts et algorithmes - De Bayes et Hume au Deep Learning*. Eyrolles.

[6] Vattenfall. (2018, 17 avril). *Pourquoi la consommation électrique varie-t-elle ?* https://www.vattenfall.fr/le-mag-energie/parametres-qui-influent-sur-la-consommation-d-electricite

---

## 🚀 Utilisation

### Prérequis

```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost jupyter
```

### Exécution des notebooks

1. Naviguez vers le dossier `code/`
2. Lancez Jupyter Notebook :
   ```bash
   jupyter notebook
   ```
3. Ouvrez les notebooks dans l'ordre suivant pour une compréhension progressive :
   - `dataset_info.ipynb` - Découverte du dataset
   - `dataset_analyse.ipynb` - Analyse exploratoire
   - `modele_statistique.ipynb` - Premiers modèles simples
   - `modele_ml_regression.ipynb` - Régressions linéaire et polynomiale
   - `modele_ml_xgb.ipynb` - Modèle XGBoost avancé
   - `modele_ml_xgb_temp.ipynb` - Modèle optimisé avec température

---

## 📈 Résultats et conclusions

Ce projet démontre l'efficacité des méthodes d'apprentissage automatique, en particulier le gradient boosting (XGBoost), pour la prédiction de consommation électrique. La prise en compte de paramètres additionnels (température, facteurs temporels) améliore significativement la précision des prédictions.

Les modèles développés permettent aux producteurs d'électricité d'optimiser leur production, de réduire les pertes énergétiques et de contribuer à une gestion plus durable de l'énergie.

---

## 👥 Auteurs

- **Téodore Autuly** - Étudiant en classe préparatoire
- **Eloi Kling** - Étudiant en classe préparatoire

---

## 📄 Licence

Ce projet a été réalisé dans le cadre d'un TIPE en classe préparatoire et est protégé par une licence MIT.

---

*Projet réalisé dans le cadre des Travaux d'Initiative Personnelle Encadrés (TIPE) - Année académique 2024-2025*
