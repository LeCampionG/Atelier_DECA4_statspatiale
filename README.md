
**Lien vers la présentation : https://lecampiong.github.io/Atelier_DECA4_statspatiale/#/title-slide** 

# Description de l’atelier

## Présentation

<!-- TODO: -->
Cet atelier propose une première initiation à la statistique spatiale avec R, pour commencer à appréhender dans l'analyse de données les effets liés à la dimension spatiale et géographique des données. Nous réaliserons un tour d’horizon des différents modèles et insisterons davantage sur ceux permettant d’étudier l’hétérogénéité spatiale des phénomènes étudiés ou comment des effets peuvent varier en fonction des lieux !
Cette réflexion sera également l’occasion d’une introduction à la réalisation de carte avec R (package mapsf) mais également avec les logiciels « clique-bouton » Magrit (<https://magrit.cnrs.fr/>) (en ligne) et Géoda (<https://geodacenter.github.io/>) pour représenter nos résultats.

## Contenu et validation :

Aucun prérequis technique n’est nécessaire (ni en statistiques, ni en R). L’atelier est pensé pour un public qui souhaite mieux comprendre les enjeux géographiques et du spatial dans l’analyse de données. Pour ce faire nous utiliserons un exemple concret visant à expliquer le prix de l’immobilier par EPCI en France Hexagonale. La validation passera par la remise d’un dossier reprenant le processus d’analyse de statistique spatiale tel qu’il aura été présenté, analyse qui pourra se baser sur des données qui auront été fournies.

## Exemple d’illustrations qui pourront être réalisées

![LISA](https://github.com/LeCampionG/deca4_2026/blob/main/images/exemple1.png?raw=true)

![collection](https://github.com/LeCampionG/deca4_2026/blob/main/images/exemple2.png?raw=true)

![nb](https://github.com/LeCampionG/deca4_2026/blob/main/images/exemple3.png?raw=true)


## Objectifs et organisation de l’atelier

### A la fin du semestre, vous saurez

-	Comprendre pourquoi et comment intégrer l’espace dans une analyse statistique
-	Utiliser de manière basique R et Magrit pour produire des cartes et des statistiques spatiales
-	Mobiliser les outils de base de la statistique spatiale (GWR, LISA)
-	Interpréter et représenter les résultats d’une analyse de statistique spatiale sur un cas réel

**Attention** cet atelier n 'est pas un atelier de cartographie des concepts essentiels comme la sémiologie graphique ne seront pas abordés mais au mieux évoqués.

### Descriptif général
<!-- PRÉCISER BASE -->
Lorsque l’on étudie des phénomènes complexes en sciences humaine et social, il est très fréquent que les effets, les explications, etc. de ces phénomènes varient en fonction du lieu. La grande question c’est pourquoi des effets des tendances sociales ou économiques observées à Paris ne sont pas les mêmes à Marseille, ou inversement ? Ce type de questions suppose en réalité de tenir compte de l’espace dans nos analyses. En tant que « pratiquant » des SHS on le conçoit intuitivement. En revanche, la statistique elle, a beaucoup plus de mal à l’appréhender. En effet, dès qu’il est question de spatial la statistique « classique » risque fort d’être inopérante.

En effet, les données spatiales posent un défi important aux modèles en statistique « classique ». Selon la première loi de la géographie formulée par Tobler – « Tout interagit avec tout, mais deux objets proches ont plus de chance de le faire que deux objets éloignés » – les données géographiques sont naturellement auto-corrélées, ce qui va à l’encontre du principe d’indépendance requis en statistique classique.
La statistique spatiale présente comme premier intérêt majeur de permettre de dépasser certaines limites de la statistique classique.
En effet, cette dépendance spatiale rend difficile l’application des modèles traditionnels, comme la régression linéaire. La statistique spatiale constitue donc une alternative à la statistique classique et permet d’intégrer la dimension spatiale à nos modèles.

Au-delà de la contrainte technique, la statistique spatiale présente un autre intérêt majeur : tenir compte du spatial nous permet plus largement de comprendre d’un point de vue statistique comment les comportements ou les dynamiques sociales peuvent varier selon les territoires ou nos voisins.
Il devient ainsi possible d’étudier l’effet des voisins sur nos individus (dépendance spatiale) ou encore d’étudier la fluctuation des effets en fonction des lieux (hétérogénéité spatiale) deux phénomènes particulièrement intéressant dans l’analyse des phénomènes en SHS.

À partir d’un exemple concret (l’analyse des prix de l’immobilier en France hexagonale), nous découvrirons des méthodes qui permettent :
-	d’identifier si des zones géographiques présentent des dynamiques similaires ou différentes (analyse LISA),
-	d’observer si les relations entre variables changent selon les lieux (régression géographiquement pondérée ou GWR),
-	et de représenter ces résultats sur des cartes claires et parlantes.

Nous utiliserons pour cela le langage R ainsi que des outils simples comme Magrit, un logiciel de cartographie en ligne et GEODA, un logiciel dédié à l'analyse de l'autocorrélation spatiale.


### Format du cours et programme prévisionnel

Les séances sont organisées en format atelier. Chaque séance comportera une dimension pratique, avec des temps d'application et exercices sur des cas concrets. Le module est organisé en séquences progressives : (1) installation de l’environnement de travail, (2) Initiation à la carto avec Magrit et Geoda, (3) Comprendre l'intérêt de la statistique spatiale, (4) réalisation de différents types d'analyse statistique spatiale ,  et (5) une ouverture vers les autres méthodes de la statistique spatiale

Bloc 1 – Mise en place & premiers pas (2 séances)  
*Objectif : permettre à chacun·e de disposer d’un environnement de travail fonctionnel*

- Présentation du cours et des attendus
- Installation des environnements de développement et prise en main
- Exécution des premières lignes de codes à partir d'un exemple fourni par l'enseignant

Ressources : [Présentation réalisé par Hugues Pecout (UMR Géographie Cité) sur R](https://introduction-59e2f5.gitpages.huma-num.fr/#/title-slide)

Bloc 2 - Initiation à Magrit (2 séances)
*Objectif : s'initier à la réalisation de cartes à laide du logiciel clic-boutons Magrit*

- Se familiariser avec l'interface
- Réaliser ses premières cartes

Bloc 3 – Pourquoi la statistique spatiale  (2 séances)  
*Objectif : comprendre l'intérêt d'utiliser la statistique spatiale*

- Comprendre la différence entre homogénéité et hétérogénéité spatiale
- Présenter un panorama des différentes méthodes de la statistique spatiale
- Comprendre pourquoi la statistique classique ne gère pas correctement la donnée spatiale
- Préparation des données pour la visualisation

Bloc 4 – Visualisation de données (5 séances)  
*Objectif : réaliser et maîtriser les principales analyses du champs de l'hétérogénéité spatiale*

- Réaliser sur R une analyse des LISA
- Réaliser 


Bloc 5 - Ouverture vers les autres méthodes de la statistique spatiale (1 séances)
*Objectif : présenter également les autres méthodes de la staistique spatiale*

- Présenter les différentes régressions spatiales
- Présenter la MGWR
- Présenter les méthodes de régionnalisation


<!-- TODO: raffiner les types de visualisation qui seront présentées -->


## Calendrier et créneaux horaire (prévisionnel)

12 séances de 1h30 

Définition en cours 


## Modes de validation

Le module propose une évaluation reposant sur la remise et la production d'un rendu final qui sera à remettre à l'issue de la dernière séance.
Le support du rendu sera fourni.

| Évaluation                                                              | Poids | Description                                        |
|---------------------------|-----------------|-----------------------------|
| QCM sur les notions qui auront été vues   | 7pts   | 1pt par bonne réponse -1pt par mauvaise réponse 0pt en cas d'absence de réponse |
| Code efficient                            | 3pts   | Un code qui se déroule sans erreur                                              |
| Analyses des statistiques                 | 5pts   | Analyse cohérentes de toutes les sorties stat des méthodes présentées           |
| Figures                                   | 3pts   | Production des visuels pertinents avec l'analyse de données                     |
| Bonus                                     | 2pts   | Proposition d'analyse plus fine que la simple sortie stat réalisé ou usages d'autres méthodes de la stat spatiale, utilisation d'autres données que celles proposées |

## Présentation des données utilisé dans le cadre de l'atelier


| Nom | Résumé | Source | Notes |
|--- |--- |--- |--- |
| data_marseille.csv | Données de pauvreté par IRIS pour Marseille (cf. détail des variables ci-dessous) | INSEE https://www.insee.fr/fr/statistiques/6049648 | Les variables explicatives ont été centrées-réduites |
| LyonIris.Rdata | Données spatiales pour l’agglomération lyonnaise (France) comprend dix variables, dont quatre environnementales (EN) et six socioéconomiques (SE) (cf. détail des variables ci-dessous) | package `geocmeans` | Fichier exporté depuis R au format Rdata |
| covid_usa.rds | données spatiales issu de l’étude de Kaashoek et al. (2022). Dans cet article, les auteures et auteurs cherchent à déterminer quels sont les facteurs socio-économiques, politiques, et sanitaires associés avec la prévalence de décès de COVID-19 dans les différents comtés des États-Unis. | Kaashoek et al. (2022) [https://www.insee.fr/fr/statistiques/6049648](https://github.com/ctesta01/spatial_poisson_covid/tree/main) |  |
| donnees_standr.csv  | Prix médian de l'immobilier par EPCI en France métropolitaine (cf. détail des variables ci-dessous) | base Notaires de France https://www.immobilier.notaires.fr/fr/prix-immobilier | Les variables explicatives ont été centrées-réduites |
| EPCI.shp  | EPCI France métropolitaine + Corse édition 2021 | IGN ADMIN-EXPRESS-COG édition 2021 par territoire https://geoservices.ign.fr/adminexpress | Les données de l'IGN ont été simplifiées avec [mapshaper]([https://mapshaper.org/) pour en réduire le poids, en utilisant l'algorithme *Visvalingam/weighted area* avec une valeur de 1 |
| IRIS13_GE.shp  | Iris recalés sur les données BD TOPO® (précision 1 m) | IGN IRIS…GE® https://geoservices.ign.fr/irisge |  |
| REGION.shp  | Nouvelles régions France métroplitaine + Corse édition 2021 | IGN ADMIN-EXPRESS-COG édition 2021 par territoire https://geoservices.ign.fr/adminexpress  | Les données de l'IGN ont été simplifiées avec [mapshaper]([https://mapshaper.org/) pour en réduire le poids, en utilisant l'algorithme *Visvalingam/weighted area* avec une valeur de 1 |

Les fichier **data_marseille.csv**, **LyonIris.Rdata** et **covid_usa.rds** seront proposé aux étudiants pour s'approprier le code et les méthodes présentées. 

**data_marseille.csv** a été constitué à partir de données de l'INSEE. Il contient les variables suivantes (attention, toutes les variables hormis le taux de bas revenu ont été centrées-réduites) :

- id_IRIS : code IRIS
- label_iris : nom de l'IRIS
- code_insee : code INSEE de la commune
- label_com : nom de la commune
- tx_bas_revenu : taux de bas revenus déclarés au seuil de 60% (%) (variable DEC_TP6019 du fichier [BASE_TD_FILO_DEC_IRIS_2019.csv](https://www.insee.fr/fr/statistiques/6049648))
- PartPop_fr : 
- hlm_res_princ : part /personne de résidences principales HLM loué vide en 2017 (%) (variable P17_RP_LOCHLMV du fichier [base-ic-logement-2017](https://www.insee.fr/fr/statistiques/4799305))
- unevoiture : part de ménages disposant au moins d'une voiture en 2017 (%) (variable P17_RP_VOIT1P du fichier [base-ic-logement-2017](https://www.insee.fr/fr/statistiques/4799305))
- res120plus : part de résidences principales de 120 m2 ou plus en 2017 (%) (variable P17_RP_120M2P du fichier [base-ic-logement-2017](https://www.insee.fr/fr/statistiques/4799305))
- masc_cadre : part d'hommes de 15 ans ou plus cadres et professions intellectuelles supérieures (%) (variable C17_H15P_CS3 du fichier [base-ic-evol-struct-pop-2017](https://www.insee.fr/fr/statistiques/4799309?sommaire=4658626))
- fem_noncadre : part de femmes de 15 ans ou plus autres sans activité professionnelle (variable C17_F15P_CS8 du fichier [base-ic-evol-struct-pop-2017](https://www.insee.fr/fr/statistiques/4799309?sommaire=4658626))

**LyonIris.Rdata** est fournit dans le package `geocmeans` développé par Jeremy Gelb et se prête bien à la réalisation de GWR, voici les différentes variables. 

- Lden : Bruit routier (Lden dB(A))
- -NO2 : Dioxyde d'azote (ug/m^3^)
- PM25 : Particules fines (PM$_{2,5}$)
- VegHautPrt : Canopée (%)
- Pct0_14 : Moins de 15 ans (%)
- Pct_65 : 65 ans et plus (%)
- Pct_Img : Immigrants (%)
- TxChom1564 : Taux de chômage
- Pct_brevet : Personnes à faible scolarité (%)
- NivVieMed : Médiane du niveau de vie (milliers d'euros)

L'unité spatiale des données est l'IRIS.Cette unité spatiale a été créee par l'INSEE afin de préparer la diffusion du recensement de la population de 1999, l'INSEE avait développé un découpage du territoire en mailles de taille homogène appelées IRIS2000. Un sigle qui signifiait « Ilots Regroupés pour l'Information Statistique » et qui faisait référence à la taille visée de 2 000 habitants par maille élémentaire.
Depuis, l'IRIS (appellation qui se substitue désormais à IRIS2000) constitue la brique de base en matière de diffusion de données infra-communales. Il doit respecter des critères géographiques et démographiques et avoir des contours identifiables sans ambigüité et stables dans le temps.
Les communes d'au moins 10 000 habitants et une forte proportion des communes de 5 000 à 10 000 habitants sont découpées en IRIS. Ce découpage constitue une partition de leur territoire. La France compte environ 16 100 IRIS dont 650 dans les DOM.
Par extension, afin de couvrir l'ensemble du territoire, on assimile à un IRIS chacune des communes non découpées en IRIS.


**covid_usa.rds** est donc issue de travaux de recherche laissé en accès libre, les variables de ce jeu de données sont regroupées en trois ensembles :

1- Variables socio-démographiques. L’hypothèse originale étant que dans les milieux plus défavorisés et moins éduqués, l’épidémie a fait plus de victimes. De même, les personnes âgées étaient particulièrement à risque pendant la pandémie, ainsi que les personnes fragilisées vivant dans des établissements de soin.

- income : niveau de revenu médian ($).
- per_black : pourcentage de la population étant afro-américaine.
- per_hispanic : pourcentage de la population étant hispanique.
- per_atleast_hs : part de la population disposant d’un diplôme de fin d’études secondaires.
- X65plus : part de la population ayant 65 ans et plus.
- per_nursing : part de la population vivant dans des établissements de soin.

2- Variables politiques. L’hypothèse originale est que certains partis politiques ont moins mis en place de mesures sanitaires ce qui a eu un impact sur le nombre de décès dans les comtés. Les comportements de la population ont aussi été affectés par les orientations politiques menant à une adoption moins systématique des gestes barrières par exemple.
  
- political_leaning : niveau d’orientation politique, calculé comme la différence entre les votes républicains (votes pour Donald Trump) et les votes démocrates (votes pour Joe Biden), divisé par le total de votants. Une valeur positive indique un état avec une tendance plus républicaine et une valeur négative indique un état à tendance plus démocrate. Ces données proviennent des données électorale du New York Times de 2020.
- strict_p3 : niveau d’intensité de mise en place de mesures sanitaires. Il s’agit d’un score développé par le Oxford COVID-19 Government Response Tracker avec des valeurs allant de 0 (absence de mesures) à 100 (mesures les plus importantes). Ces données sont obtenues à l’échelle des États.
  
3- Variables de contagion. Plusieurs facteurs expliquent la propagation de la maladie tels que la proximité aux aéroports, les niveaux de mobilité dans les comtés ou encore le port du masque.

- density : densité de population du comté.
- google_p3 : niveaux de mobilité pour le motif du travail selon les données de Google Mobility. Cet indicateur est comparatif par rapport à une tendance habituelle et est exprimé en pourcentage. Une mobilité plus importante serait associée à une moins bonne distanciation sociale entre individus de ménages différents.
- dist_to_airport : la distance à l’aéroport internationnal le plus proche.
- mask_usage_p3 : estimation de la proportion des personnes portant le masque la plupart du temps ou tout le temps en public. Ces données proviennent d’une enquête effectuée par Facebook (Facebook’s COVID-19 symptom survey).


Les données utilisés en présentation et en exemple ont été constitué par Frédéric Audard et Alice Ferrari à partir de la base Notaires de France. Il contient les variables suivantes (attention, toutes les variables hormis le prix médian ont été centrées-réduites) :

- SIREN : code SIREN de l'EPCI
- prix_med : pris médian par EPCI à la vente
- perc_log_vac : % logements vacants
- perc_maison : % maisons
- perc_tiny_log : % petits logements
- dens_pop : densité de population
- med_niveau_vis : médiane du niveau de vie
- part_log_suroccup : % logements suroccupés
- part_agri_nb_emploi : % agriculteurs
- part_cadre_profintellec_nbemploi : % cadres et professions intellectuelles

Ces données sont à l'échelle de l'EPCI (établissements publics de coopération intercommunale). Les EPCI sont des structures administratives permettant à plusieurs communes d’exercer des compétences en commun.
Ils sont soumis à des règles communes, homogènes et comparables à celles de collectivités locales. Les communautés urbaines, communautés d'agglomération, communautés de communes, syndicats d'agglomération nouvelle, syndicats de communes et les syndicats mixtes sont des EPCI.
(source INSEE)


### Bibliographie / Ressources

<!-- TODO : COMPLÉTER LA BIBLIO -->
- Hugues Pecout (CNRS, UMR Géographie-Cités), 2024. Introduction à R. Formation Interne - Transversalité "Données et protocoles dans les Humanités Numériques". [Consultable ici](https://gitlab.huma-num.fr/geographie-cites/formation/inititation-r/introduction/-/tree/master?ref_type=heads)
- Lien vers Geoda : https://geodacenter.github.io/
- Lien vers Magrit : https://magrit.cnrs.fr/
- Tuto stat spatiale : Consultable ici](https://letg.pages.in2p3.fr/initiation-formation-aux-statistiques-spatiales/ifoss_immo.html#pour-aller-plus-loin-la-gwr-multiscalaire-et-r%C3%A9gionalisation)





## À propos de l’enseignant-e
<!-- TODO :  -->

Grégoire Le Campion est ingénieur d'études au CNRS en traitement et analyse de bases de données au sein de l'UMR Passages.
