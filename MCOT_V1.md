# MCOT

## Titres possibles :

- Prévisions de la conservation électrique.

- Optimisation de la conservation d'énergie électrique par la prévision de consommation électrique.

- Des applications d'intelligence artificielle pour prédire la consommation électrique. (C'est littéralement ce qu'on fait, mais il manque la partie sur les objectifs sous jacents, ce qui n'est pas forcément un problème tant qu'on en parle juste après)

- Prévoir la consommation électrique pour favoriser une distribution énergétique optimale.

Motivation du choix de l'étude : (49 mots)

De nos jours, toute énergie électrique produite en excès est soit stockée, soit perdue. Cependant, le stockage de l'électricité rencontre de nombreux problèmes d'efficacité. Les producteurs d’électricité utilisent donc des modèles prédictifs destinés à ajuster la production d’énergie en fonction de la demande afin de limiter le gaspillage énergétique.

Ancrage au thème de l'année : (47 mots)

La consommation électrique des villes suit des comportements prévisibles et normalisés par la multitude de consommateurs, alors que celle des foyers isolés est imprévisible, voire chaotique. C'est pourquoi les modèles prédictifs en jeu sont uniquement entraînés sur des bases de données répertoriant la consommation électrique des villes.

#### I Positionnements thématiques et *mots-clés*

**<u>Position thématique:</u>** INFORMATIQUE (Informatique pratique), INFORMATIQUE (Informatique théorique).

| Mots clés Français        | Mots clés Anglais          |
| ------------------------- | -------------------------- |
| Optimisation              | Optimization               |
| Apprentissage automatique | Machine learning           |
| Renforcement de gradient  | Gradient boosting(XGboost) |
| Base de donnée            | Database                   |
| Pandas                    | Pandas                     |

#### II Bibliographie commentée

Plan :

1. Explications des difficultés à stocker l'énergie en citant l'article d'EDF.

2. Ce que l'informatique, en particulier le machine learning, permet d'apporter comme plus-value dans le secteur de l'énergie.

3. Explication du machine learning et des modèles.

4. XGBoost en citant le livre *Apprentissage Artificiel*.

5. Ajout des paramètres (température, etc...) pour plus de précision et d'optimisation.

#### Bibliographie commentée (642 mots)

De nos jours, le stockage de l'énergie électrique permet d'ajuster la production électrique à la consommation par les usagers. En effet, l'électricité produite en surcroît lors des périodes de creux est stockée pour être utilisée ultérieurement lors d'une période de consommation plus élevée.

Cependant, les technologies actuelles ne permettent pas de stocker l'électricité telle qu'elle. Les méthodes de stockage consistent aujourd'hui à convertir un courant électrique en une autre forme d’énergie stockable, ce qui soulève de nouvelles problématiques environnementales et d'efficacité. En effet, ces conversions énergétiques sont coûteuses financièrement, elle provoquent des pertes énergétiques et détériorent l'environnement (bétonnage dû aux barrages hydrauliques, stockage électrochimique etc...) [1]

Il est donc préférable dans la mesure du possible d'éviter toute forme de stockage d'énergie et de s'intéresser à l'optimisation de la production énergétique afin de limiter le gaspillage d'énergie électrique. Pour ce faire, il faut être capable de produire de l'électricité de manière ajustée par rapport à la consommation électrique des usagers. Il est donc nécessaire de connaître à l'avance la demande électrique pour ajuster la production. L’intelligence artificielle (IA), notamment par sa capacité à prédire, a un rôle à jouer dans la solution à ces défis. Les outils d'intelligence artificielle sont amenés à prendre une part grandissante dans les secteurs de l’énergie à mesure que les systèmes se décentralisent et se complexifient. L'essort des sources d'énergie intermmitentes, en particulier les énergies renouvelables, renforce ce besoin d'optimiser la production énergétique. Aujourd'hui les applications d'intelligence artificielle indispensables sont donc indispensables à la transition énergétique. [2]

Le premier atout de l’apprentissage automatique (machine learning) est qu’il permet de prédire un comportement futur à partir d'un comportement passé connu dont les données sont répertoriées dans une base de donnée. De plus, les données de consommation énergétique sont précises et accessibles en grande quantité grâce aux nouvelles technologies de compteur électrique (commes les compteurs automatiques, compteurs linky), ce qui permet d'alimenter efficacement les modèles de machine learning et d'implémenter plus facilement des modèles prédictifs de la consommation. [2]

Le Machine Learning consiste à faire apprendre aux ordinateurs à exécuter trois types d’actions : prédire, classifier et regrouper.

Les algorithmes ou modèles effectuant ces tâches sont appelés respectivement:

- Des **régressions**: Ridge, Lasso, forêt d’arbres décisionnels, gradient boosting, réseaux de neurones, etc.

- Des **classificateurs** : machine à vecteurs de support, arbres décisionnels, réseaux de neurones etc.

- Des algorithmes de **partitionnement de données** ou **clustering** (apprentissage non supervisé) : k-means, etc.[3]

Dans le cas de la prédiction de consommation électrique, les modèles ont un but purement prédictif, ce sont des problèmes de régression.

Les modèles de machine learning permettant de répondre à ces problèmes sont nombreux : Modèle polynomial, statistique, régression linéaire etc...

Cependant, le modèle le plus performant aujourd'hui est le boosting de gradient, qui a fait ses preuves en terme de performance et de vitesse d'exécution pour résoudre des problèmes de régression. Ce modèle consiste à construire successivement des arbres de décision en favorisant la correction des données les moins bien prédites à chaque construction.[4] C'est une méthode d'apprentissage d'ensemble, qui forme plusieurs modèles individuels et indépendants, entraînés pour un objectif propre, puis les combine afin de créer un modèle plus fort qui permet de résoudre tous les objectifs de chaque modèle fusionnés. [5]

La prise en compte de nombreux facteurs est essentielle à la prédiction de la consommation électrique. Les paramètres temporels, saisonniers, météorologiques, conjoncturels apportent des informations importantes sur les tendances de consommation. C’est pourquoi des modèles toujours plus fins sont mis au point en prenant en compte toujours plus de paramètres pour permettre des prédictions les plus précises possibles. Les principales applications d'intelligence artificelle appliquées dans le secteur de l'énergie nécessitent une base de donnée contenant l'heure de la mesure de la consommation ainsi que la température extérieure dans la zone concernée, mais il est possible de prendre en compte d'autres paramètres significatifs.

#### III Problématique retenue (49 mots)

Notre sujet a pour but de répondre aux problématiques suivantes : Comment prévoir efficacement la consommation électrique à venir ? Sur quelle base de donnée ? Quels modèles de machine learning sont judicieux pour cette étude ? Comment fonctionnent-ils ? Quels sont les paramètres prédominants affectant les données ?

#### IV Objectifs du TIPE: (99 mots)

 - Trouver une base de données adaptée à notre problème et la mettre en forme.

 - Réaliser un premier modèle simple, statistique, pour obtenir de premiers résultats à critiquer.

 - Réaliser des modèles de machine learning (régréssion lineaire et polynomial) et confronter les prédictions des modèles entre eux.

 - Réaliser enfin un modèle plus fin de machine learning en utilisant la méthode du gradient boosting.

 - Étudier les aspects théorique et mathématique du gradient boosting.

 - S'appliquer sur une autre base de donnée et réaliser un modèle de machine learning en prenant en compte de nouveaux paramètres puis conclure.

1. Objectifs du TIPE de Eloi:

2. Objectifs du TIPE de Téodore: (Le partage des objectifs n'a pas encore été fait)

#### V Listes de références bibliographiques

[1] EDF. (2021, 14 décembre). *Tout savoir sur le stockage de l’électricité*. https://particulier.edf.fr/fr/accueil/guide-energie/electricite/stockage-energie-electricite.html

[2] *Machine learning appliqué au domaine de l’énergie — CultureSciences-Physique - Ressources scientifiques pour l’enseignement des sciences physiques*. (s. d.). https://culturesciencesphysique.ens-lyon.fr/ressource/IA-energie-Delinchant.xml

[3] Moogsoft. (2019, 16 octobre). *Understanding the Machine Learning in AIOps*. Industry Leading AIOps and Observability Platform for IT Ops and DevOps. https://www.moogsoft.com/resources/aiops/white-paper/understanding-machine-learning

[4] *XGBoost : Tout savoir sur le Boosting*. (s. d.). Formations Data & ; Tech - Blent.ai.

https://blent.ai/xgboost-tout-comprendre/

[5] Barra, V., Miclet, L. & Cornuéjols, A. (2021). *Apprentissage artificiel - 4e édition : Concepts et algorithmes - De Bayes et Hume au Deep Learning*. Eyrolles.
