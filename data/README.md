#  Dossier `data/`

Ce dossier contient les **jeux de données** utilisés tout au long du cours **Introduction à la Data Science**.  
Chaque dataset permet de mettre en pratique les notions abordées dans les chapitres : collecte, exploration, visualisation et modélisation.

---

##  Structure du dossier

```
data/
│
├── titanic.csv                # Données des passagers du Titanic
├── netflix_titles.csv         # (à venir) Données sur les films et séries Netflix
├── housing.csv                # (à venir) Données sur les prix de l'immobilier
└── README.md                  # Description des datasets
```

---

##  Dataset principal : Titanic

**Nom du fichier :** `titanic.csv`  
**Source :** [DataScienceDojo / Kaggle](https://www.kaggle.com/datasets/heptapod/titanic)  
**Lien brut :** [https://raw.githubusercontent.com/datasciencedojo/datasets/master/titanic.csv](https://raw.githubusercontent.com/datasciencedojo/datasets/master/titanic.csv)

### Description

Le dataset Titanic contient des informations sur les passagers du célèbre paquebot.  
Il est utilisé pour introduire la collecte, le nettoyage, l’exploration et la modélisation des données.

| Colonne | Description |
|----------|-------------|
| `PassengerId` | Identifiant du passager |
| `Survived` | 1 = a survécu, 0 = n’a pas survécu |
| `Pclass` | Classe du billet (1, 2, 3) |
| `Name` | Nom du passager |
| `Sex` | Sexe |
| `Age` | Âge |
| `SibSp` | Nombre de frères/sœurs ou conjoints à bord |
| `Parch` | Nombre de parents/enfants à bord |
| `Ticket` | Numéro de ticket |
| `Fare` | Prix du billet |
| `Cabin` | Numéro de cabine (souvent manquant) |
| `Embarked` | Port d’embarquement (C = Cherbourg, Q = Queenstown, S = Southampton) |

---
#  Sources de données ouvertes pour la Data Science

Voici une liste de plateformes et de ressources où vous pouvez télécharger ou explorer des **datasets gratuits** pour vos projets de Data Science, en complément du dataset Titanic.

---

##  Plateformes généralistes


| **Kaggle Datasets** | La plus grande communauté de Data Science. Contient des milliers de datasets prêts à l'emploi (CSV, JSON, images, etc.). | [https://www.kaggle.com/datasets](https://www.kaggle.com/datasets) |
| **Google Dataset Search** | Moteur de recherche mondial de datasets publiés en ligne. | [https://datasetsearch.research.google.com/](https://datasetsearch.research.google.com/) |
| **UCI Machine Learning Repository** | Datasets classiques utilisés dans la recherche et l’enseignement (Iris, Wine, Spam, etc.). | [https://archive.ics.uci.edu/ml/index.php](https://archive.ics.uci.edu/ml/index.php) |
| **DataCamp Datasets** | Petits jeux de données pour l’apprentissage interactif. | [https://www.datacamp.com/datasets](https://www.datacamp.com/datasets) |
| **Awesome Public Datasets (GitHub)** | Liste communautaire de centaines de datasets regroupés par domaine. | [https://github.com/awesomedata/awesome-public-datasets](https://github.com/awesomedata/awesome-public-datasets) |

---

##  Sources francophones et open data

| Source | Description | Lien |
|--------|--------------|------|
| **data.gouv.fr** | Portail officiel français d’open data (santé, transports, énergie, éducation, etc.). | [https://www.data.gouv.fr](https://www.data.gouv.fr) |
| **INSEE Open Data** | Données économiques, démographiques et sociales officielles. | [https://www.insee.fr/fr/statistiques](https://www.insee.fr/fr/statistiques) |
| **OpenDataSoft** | Plateforme française d’open data multi-domaines. | [https://www.opendatasoft.com](https://www.opendatasoft.com) |
| **Banque mondiale (World Bank Data)** | Données globales sur le développement économique et social. | [https://data.worldbank.org/](https://data.worldbank.org/) |
| **OECD Data** | Statistiques internationales (économie, emploi, environnement, etc.). | [https://data.oecd.org/](https://data.oecd.org/) |

---

## Datasets éducatifs pour l’enseignement

| Nom | Description | Lien |
|------|--------------|------|
| **Iris Dataset** | Classique pour apprendre la classification supervisée. | [Lien UCI](https://archive.ics.uci.edu/ml/datasets/iris) |
| **Wine Quality** | Qualité de vins portugais, utilisé pour la régression. | [Lien UCI](https://archive.ics.uci.edu/ml/datasets/wine+quality) |
| **Students Performance** | Scores d’examens selon le sexe, la préparation, etc. | [Lien Kaggle](https://www.kaggle.com/spscientist/students-performance-in-exams) |
| **Netflix Movies** | Données sur les films/séries Netflix (titre, genre, pays, etc.). | [Lien Kaggle](https://www.kaggle.com/shivamb/netflix-shows) |
| **Housing Prices** | Données sur les prix de logements à Boston ou Ames. | [Lien Kaggle](https://www.kaggle.com/c/house-prices-advanced-regression-techniques) |
| **Covid-19 Data** | Statistiques mondiales et régionales de la pandémie. | [Lien John Hopkins](https://github.com/CSSEGISandData/COVID-19) |

---

##  Datasets spécialisés par domaine

### 🔹 Économie et société
- [IMF Data](https://data.imf.org/) — Fonds monétaire international  
- [Eurostat](https://ec.europa.eu/eurostat/web/main/data/database) — Données de l’Union européenne  
- [Our World in Data](https://ourworldindata.org/) — Indicateurs mondiaux (éducation, santé, énergie, etc.)

### 🔹 Santé
- [WHO Global Health Observatory](https://www.who.int/data/gho) — Statistiques de santé mondiales  
- [Open Food Facts](https://world.openfoodfacts.org/) — Données sur les produits alimentaires  

### 🔹 Environnement
- [NASA Earth Data](https://earthdata.nasa.gov/) — Données environnementales et climatiques  
- [NOAA Climate Data Online](https://www.ncdc.noaa.gov/cdo-web/) — Données climatiques américaines  

### 🔹 Technologie et médias
- [GitHub Archive](https://www.gharchive.org/) — Données issues des événements GitHub publics  
- [IMDb Datasets](https://datasets.imdbws.com/) — Données sur les films, séries et acteurs  

---

##  Astuce pour charger un dataset depuis une URL

```python
import pandas as pd

url = "https://raw.githubusercontent.com/datasciencedojo/datasets/master/titanic.csv"
df = pd.read_csv(url)
df.head()
```


## Utilisation dans les notebooks

Pour charger le dataset directement depuis le dossier `data/` :

```python
import pandas as pd

df = pd.read_csv("data/titanic.csv")
df.head()
```

Ou depuis GitHub (sans téléchargement manuel) :

```python
url = "https://raw.githubusercontent.com/<TON_UTILISATEUR>/<TON_REPO>/main/data/titanic.csv"
df = pd.read_csv(url)
```

> 🔁 Remplace `<TON_UTILISATEUR>` et `<TON_REPO>` par ton nom d’utilisateur et le nom du dépôt GitHub.

---

 Bonnes pratiques

- Ne jamais modifier les fichiers de données brutes directement.  
- Créer un dossier séparé (`/processed` ou `/cleaned`) pour les versions nettoyées.  
- Toujours documenter la source et la transformation des données.

  


