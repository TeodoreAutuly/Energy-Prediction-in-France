# MCOT

## Titre : Prévisions de la consommation d'énergie électrique à l'aide de méthodes d'apprentissage.

Motivation du choix de l'étude :

(Version corrigée 50 mots) De nos jours, toute énergie électrique produite en excès encourt des pertes importantes. C'est pourquoi notre intérêt est de mettre au point des modèles prédictifs destinés à anticiper la consommation électrique. De cette manière, les producteurs d'électricité peuvent ajuster la production à la demande prévue afin de limiter les pertes.

Ancrage au thème de l'année :

(Version corrigée 50 mots) Les modèles prédictifs en jeu ne sont efficaces que pour prédire la consommation électrique des villes qui suit des comportements tendanciels et normalisés par la multitude de consommateurs. De surcroît, les prévisions réalisées favorisent alors une production d'électricité à proximité des villes, réduisant les pertes dûes au transport de l'énergie.

#### I Positionnements thématiques et *mots-clés*

**<u>Position thématique:</u>** INFORMATIQUE (Informatique pratique), INFORMATIQUE (Informatique théorique).

| Mots clés Français         | Mots clés Anglais          |
| -------------------------- | -------------------------- |
| Optimisation               | Optimization               |
| Apprentissage automatique  | Machine learning           |
| Renforcement de gradient   | Gradient boosting(XGBoost) |
| Base de donnée             | Database                   |
| Bibliothèque Python Pandas | Python Library Pandas      |

#### II Bibliographie commentée

Plan : (Ne sera pas présent sur le document final)

1. Explications des difficultés à stocker l'énergie en citant l'article d'EDF.

2. Ce que l'informatique, en particulier le machine learning, permet d'apporter comme plus-value dans le secteur de l'énergie.

3. Explication du machine learning et des modèles.

4. XGBoost en citant le livre *Apprentissage Artificiel*.

5. Ajout des paramètres (température, etc...) pour plus de précision et d'optimisation.

#### Bibliographie commentée (646 mots)

De nos jours, le stockage de l'énergie électrique permet d'ajuster la production électrique à la consommation des usagers. En effet, l'électricité produite en surcroît lors des périodes de creux est stockée pour être utilisée ultérieurement lors d'une période de consommation plus élevée.

Cependant, les technologies actuelles ne permettent pas de stocker l'électricité telle qu'elle. Les méthodes de stockage consistent aujourd'hui à convertir un courant électrique en une autre forme d’énergie stockable, ce qui soulève de nouvelles problématiques environnementales et financières. En plus d'être coûteuses financièrement, ces conversions provoquent des pertes énergétiques et détériorent l'environnement avec le bétonnage dû à l'implémentation de nouveaux barrages hydrauliques par exemple. [1]

Il est donc préférable dans la mesure du possible d'éviter toute forme de stockage d'énergie et de s'intéresser à l'optimisation de la production énergétique afin de limiter le gaspillage d'énergie électrique. Pour ce faire, il faut être capable de produire de l'électricité de manière ajustée par rapport à la consommation électrique des usagers. Il est donc nécessaire de connaître à l'avance la demande pour ajuster la production. En ce sens, l’intelligence artificielle (IA) -un ensemble de techniques qui permettent de simuler le comportement d'une intelligence humaine- est particulièrement efficace pour prédire ces données de consommation. Les méthodes d'apprentissage sont donc amenées à prendre une part grandissante dans les secteurs de l’énergie à mesure que les systèmes se décentralisent et se complexifient. L'essort des sources d'énergie intermmitentes, en particulier les énergies renouvelables, renforce ce besoin d'optimiser la production énergétique. Aujourd'hui les applications de méthodes d'apprentissage sont donc indispensables à la transition énergétique. [2]

Le premier atout de l’apprentissage automatique (machine learning) est qu’il permet de prédire un comportement futur à partir d'un comportement passé connu dont les données sont répertoriées dans une base de donnée. De plus, les données de consommation énergétique sont précises et accessibles en grande quantité grâce aux nouvelles technologies de compteur électrique (commes les compteurs automatiques, compteurs linky), ce qui permet d'alimenter efficacement les modèles de machine learning et d'implémenter plus facilement des modèles prédictifs de la consommation. [2]

L'apprentissage automatique consiste à faire apprendre aux ordinateurs à exécuter trois types d’actions : prédire, classifier et regrouper.

Les algorithmes ou modèles effectuant ces tâches sont appelés respectivement:

- Des **régressions**: Ridge, forêt d’arbres décisionnels, gradient boosting, réseaux de neurones etc...

- Des **classificateurs** : k plus proches voisins, arbres de décision, réseaux de neurones, ID3 etc...

- Des algorithmes de **partitionnement de données** ou **clustering** (apprentissage non supervisé) : k-means etc...[3]

Dans le cas de la prédiction de consommation électrique, les modèles ont un but purement prédictif, ce sont des problèmes de régression.

Les modèles de machine learning permettant de répondre à ces problèmes sont nombreux : Régression linéaire, polynomial, statistique etc...

Cependant, le modèle le plus performant aujourd'hui est le renforcement de gradient, qui a fait ses preuves en terme de performance et de vitesse d'exécution pour résoudre des problèmes de régression. Ce modèle consiste à construire successivement de nouvelles feuilles à un arbre de décision en favorisant la correction des données les moins bien prédites à chaque construction.[4] C'est une méthode d'apprentissage d'ensemble, c'est-à-dire qu'elle forme plusieurs modèles individuels et indépendants, entraînés pour un objectif propre, puis les combine afin de créer un modèle plus fort satisfaisant tous les objectifs. [5]

La prise en compte de nombreux facteurs est essentielle à la prédiction de la consommation électrique, comme les paramètres temporels, saisonniers, météorologiques, économiques ou conjoncturels. [6] C’est pourquoi des modèles toujours plus fins sont mis au point en prenant en compte toujours plus de paramètres pour permettre des prédictions les plus précises possibles. Les principales applications d'intelligence artificelle appliquées dans le secteur de l'énergie nécessitent une base de donnée contenant l'heure de la mesure de la consommation ainsi que la température extérieure dans la zone concernée, mais il est possible de prendre en compte d'autres paramètres significatifs.

De là se dégage plusieurs problématiques.

#### III Problématique retenue (39 mots)

Notre avons retenu une problématique synthétisant tous les questionnements sur lesquels nous nous sommes penchés au cours de notre étude : Quelles sont les méthodes d'apprentissage les plus efficaces pour prévoir la consommation d'énergie électrique de manière optimisée ?

#### IV Objectifs du TIPE: (98 mots)

 - Utiliser et mettre en forme une base de données adaptée à notre problème.

 - Réaliser des modèles naïfs de machine learning (statistique, régréssion lineaire et polynomial) et confronter les prédictions des modèles entre eux.

 - Réaliser enfin un modèle plus fin de machine learning en utilisant la méthode du renforcement de gradient.

 - Comparer les méthodes entre elles.

 - Étudier les aspects théoriques du gradient boosting.

 - Utiliser une autre base de donnée et réaliser un modèle de machine learning en prenant en compte de nouveaux paramètres.

 - Etudier l'importance des paramètres en faisant varier leur utilisation.

1. Objectifs du TIPE de Eloi:
2. Objectifs du TIPE de Téodore: (Le partage des objectifs n'a pas encore été fait)

#### V Listes de références bibliographiques

[1] EDF. (2021, 14 décembre). *Tout savoir sur le stockage de l’électricité*. https://particulier.edf.fr/fr/accueil/guide-energie/electricite/stockage-energie-electricite.html

[2] Pierre-Thomas Demars, Vincent Imard, Benoît Delinchant. *Machine learning appliqué au domaine de l’énergie — CultureSciences-Physique - Ressources scientifiques pour l’enseignement des sciences physiques*. (s. d.). https://culturesciencesphysique.ens-lyon.fr/ressource/IA-energie-Delinchant.xml

[3] Moogsoft. (2019, 16 octobre), Robert Harper. *Understanding the Machine Learning in AIOps*. Industry Leading AIOps and Observability Platform for IT Ops and DevOps. https://www.moogsoft.com/resources/aiops/white-paper/understanding-machine-learning

[4] Formations Data & ; Tech - Blent.ai. (2022, 4 Février), Nada Belaidi. *XGBoost : Tout savoir sur le Boosting*. (s. d.).

https://blent.ai/xgboost-tout-comprendre/

[5] Barra, V., Miclet, L. & Cornuéjols, A. (2021). *Apprentissage artificiel - 4e édition : Concepts et algorithmes - De Bayes et Hume au Deep Learning*. Eyrolles.

[6] Vattenfall. (2018, 17 avril). *Pourquoi la consommation électrique varie-t-elle ?*

https://www.vattenfall.fr/le-mag-energie/parametres-qui-influent-sur-la-consommation-d-electricite
