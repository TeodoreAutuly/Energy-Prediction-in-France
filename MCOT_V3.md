# MCOT

## Titre : Prévisions de la consommation d'énergie électrique à l'aide de méthodes d'apprentissage.

De nos jours, toute énergie électrique produite en excès encourt des pertes importantes. C'est pourquoi notre intérêt est de mettre au point des modèles prédictifs destinés à anticiper la consommation électrique. De cette manière, les producteurs d'électricité peuvent ajuster la production à la demande prévue afin de limiter les pertes.

Les modèles prédictifs en jeu ne sont efficaces que pour prédire la consommation électrique des villes qui suit des comportements tendanciels et normalisés par la multitude de consommateurs. De surcroît, les prévisions réalisées favorisent alors une production d'électricité à proximité des villes, réduisant les pertes dues au transport de l'énergie.

#### I Positionnements thématiques et *mots-clés*

**<u>Position thématique:</u>** INFORMATIQUE (Informatique pratique), INFORMATIQUE (Informatique théorique).

| Mots clés Français         | Mots clés Anglais          |
| -------------------------- | -------------------------- |
| Optimisation               | Optimization               |
| Apprentissage automatique  | Machine learning           |
| Renforcement de gradient   | Gradient boosting(XGBoost) |
| Base de données            | Database                   |
| Bibliothèque Python Pandas | Python Library Pandas      |

#### II Bibliographie commentée

Plan : (Ne sera pas présent sur le document final)

1. Explications des difficultés à stocker l'énergie en citant l'article d'EDF.

2. Ce que l'informatique, en particulier le machine learning, permet d'apporter comme plus-value dans le secteur de l'énergie.

3. Explication du machine learning et des modèles.

4. XGBoost en citant le livre *Apprentissage Artificiel*.

5. Ajout des paramètres (température, etc...) pour plus de précision et d'optimisation.

#### Bibliographie commentée

De nos jours, le stockage de l'énergie électrique permet d'ajuster la production électrique à la consommation des usagers. En effet, l'électricité produite en surcroît lors des périodes de creux est stockée pour être utilisée ultérieurement lors d'une période de consommation plus élevée.

Cependant, les technologies actuelles ne permettent pas d'emmagasiner l'électricité telle qu'elle. Les méthodes de conservation consistent aujourd'hui à convertir un courant électrique en une autre forme d’énergie conservable, ce qui soulève de nouvelles problématiques environnementales et financières. En plus d'être coûteuses, ces conversions provoquent des pertes énergétiques et détériorent l'environnement avec le bétonnage dû à l'implémentation de nouveaux barrages hydrauliques par exemple. [1]

Il est donc préférable de s'intéresser à l'optimisation de la production énergétique afin de limiter le gaspillage d'énergie électrique. Pour ce faire, il faut être capable de produire de l'électricité de manière ajustée par rapport à la consommation électrique des usagers. Il est donc nécessaire de connaître à l'avance la demande pour ajuster la production. En ce sens, l’intelligence artificielle (IA) -un ensemble de techniques qui permettent de simuler le comportement d'une intelligence humaine- est particulièrement efficace pour prédire ces données de consommation. Les méthodes d'apprentissage sont donc amenées à prendre en importance dans les secteurs de l’énergie à mesure que les systèmes gagnent en complexité et se décentralisent. L'essor des sources d'énergie intermittentes, en particulier les énergies renouvelables, renforce ce besoin d'optimiser la production énergétique. [2]

Le premier atout de l’apprentissage automatique (machine learning) est qu’il permet de prédire un comportement futur à partir d'un comportement passé connu dont les informations sont répertoriées dans une base de données. De plus, les relevés de consommation énergétique sont précis et accessibles en grande quantité grâce aux nouvelles technologies de compteur électrique (comme les compteurs automatiques), ce qui permet d'alimenter efficacement les modèles de machine learning et d'implémenter plus facilement des modèles prédictifs de la consommation. [2]

L'apprentissage automatique consiste à faire apprendre aux machines à réaliser trois types d’actions : prédire, classifier et regrouper.

Les algorithmes ou modèles effectuant ces tâches sont appelés respectivement :

- Des **régressions** : Forêt d’arbres décisionnels, gradient boosting, réseaux de neurones ...

- Des **classificateurs** : k plus proches voisins, arbres de décision, réseaux de neurones, ID3 ...

- Des algorithmes de **partitionnement de données** ou **clustering** (apprentissage non supervisé) : k-means ... [3]

Dans le cas de la prédiction de consommation électrique, les modèles ont un but purement prédictif, ce sont des problèmes de régression.

Les modèles de machine learning permettant de répondre à ces problèmes sont nombreux : Régression linéaire, polynomial, statistique etc...

Pour résoudre des problèmes de régression, le modèle le plus performant aujourd'hui est le renforcement de gradient. Ce modèle consiste à construire successivement de nouvelles feuilles à un arbre de décision en favorisant la correction des données les moins bien prédites à chaque construction.[4] C'est une méthode d'apprentissage d'ensemble, c'est-à-dire qu'elle forme plusieurs modèles individuels et indépendants, entraînés pour un objectif propre, puis les combine afin de créer un modèle plus fort satisfaisant tous les objectifs. [5]

La prise en compte de nombreux facteurs est essentielle à la prédiction de la consommation électrique, comme les paramètres temporels, saisonniers, météorologiques, économiques ou conjoncturels. [6] C’est pourquoi des modèles toujours plus fins sont mis au point en prenant en compte toujours plus de paramètres pour permettre des prédictions les plus précises possibles. Les principales applications d'intelligence artificielle dans le secteur de l'énergie nécessitent une base de données contenant l'heure de la mesure de la consommation ainsi que la température extérieure dans la zone concernée, mais il est possible de prendre en compte d'autres paramètres significatifs.

#### III Problématique retenue

Quelles sont les méthodes d'apprentissage les plus efficaces pour prévoir la consommation d'énergie électrique ?

#### IV Objectifs Téodore

 - Utiliser et mettre en forme une base de données adaptée à notre problème.

 - Réaliser des modèles naïfs de machine learning statistique et linéaire puis confronter les prédictions des modèles entre eux.

 - Comparer les méthodes entre elles.

 - Étudier les aspects théoriques du gradient boosting.

 - Utiliser une autre base de données et réaliser un modèle de machine learning en prenant en compte de nouveaux paramètres.

#### IV Objectifs Eloi

 - Utiliser et mettre en forme une base de données adaptée à notre problème.

 - Réaliser des modèles naïfs de machine learning statistique et polynomial puis confronter les prédictions des modèles entre eux.

 - Réaliser enfin un modèle plus fin de machine learning en utilisant la méthode du renforcement de gradient.

 - Comparer les méthodes entre elles.

 - Etudier l'importance des nouveaux paramètres pris en compte en faisant varier leur utilisation.

#### V Listes de références bibliographiques

[1] EDF. (2021, 14 décembre). *Tout savoir sur le stockage de l’électricité*. https://particulier.edf.fr/fr/accueil/guide-energie/electricite/stockage-energie-electricite.html

[2] Pierre-Thomas Demars, Vincent Imard, Benoît Delinchant. *Machine learning appliqué au domaine de l’énergie — CultureSciences-Physique - Ressources scientifiques pour l’enseignement des sciences physiques*. https://culturesciencesphysique.ens-lyon.fr/ressource/IA-energie-Delinchant.xml

[3] Moogsoft. (2019, 16 octobre), Robert Harper. *Understanding the Machine Learning in AIOps*. Industry Leading AIOps and Observability Platform for IT Ops and DevOps. https://www.moogsoft.com/resources/aiops/white-paper/understanding-machine-learning

[4] Formations Data & ; Tech - Blent.ai. (2022, 4 Février), Nada Belaidi. *XGBoost : Tout savoir sur le Boosting*.

https://blent.ai/xgboost-tout-comprendre/

[5] Barra, V., Miclet, L. & Cornuéjols, A. (2021). *Apprentissage artificiel - 4e édition : Concepts et algorithmes - De Bayes et Hume au Deep Learning*. Eyrolles.

[6] Vattenfall. (2018, 17 avril). *Pourquoi la consommation électrique varie-t-elle ?*

https://www.vattenfall.fr/le-mag-energie/parametres-qui-influent-sur-la-consommation-d-electricite
