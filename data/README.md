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


