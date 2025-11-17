#  Notebooks — Introduction à la Data Science

Ce dossier contient les notebooks Jupyter utilisés dans le cadre du cours **Introduction à la Data Science**.  
Chaque notebook correspond à un chapitre du cours : exploration, visualisation, machine learning, etc.

---

##  Installation locale

### 1️ Créer un environnement virtuel

Il est recommandé d’utiliser un environnement Python isolé pour exécuter les notebooks :

```bash
# Sous macOS / Linux
python3 -m venv notebooksvenv
source notebooksvenv/bin/activate

# Sous Windows
python -m venv venv
venv\Scripts\activate
```

---

### 2️ Installer les dépendances

Une fois l’environnement activé, installez les bibliothèques nécessaires :

```bash
pip install -r requirements.txt
```

Le fichier **requirements.txt** contient les dépendances suivantes :

- pandas  
- numpy  
- matplotlib  
- seaborn  
- scikit-learn  
- jupyter

---

### 3️ Lancer Jupyter Notebook ou JupyterLab

```bash
jupyter notebook
# ou
jupyter lab
```

Puis ouvrez le notebook correspondant au chapitre, par exemple :

```
notebooks/Chapitre_1_Introduction.ipynb
```

---

##  Utilisation avec Google Colab (optionnel)

Si vous ne souhaitez pas installer Python localement, vous pouvez exécuter les notebooks directement dans **Google Colab** :

1. Ouvrez le notebook sur GitHub.  
2. Cliquez sur le bouton **“Open in Colab”** ou utilisez un lien comme celui-ci :

```
https://colab.research.google.com/github/<TON_UTILISATEUR>/Introduction-to-Data-Science/blob/main/notebooks/Chapitre_1_Introduction.ipynb
```

 *Pensez à monter votre Google Drive si vous souhaitez sauvegarder vos modifications.*

---

##  Structure du dossier

```
notebooks/
│
├── Chapitre_1_Introduction.ipynb
├── Chapitre_2_Collecte_et_stockage.ipynb
├── Chapitre_3_Exploration_et_visualisation.ipynb
├── Chapitre_4_Machine_Learning.ipynb
├── Chapitre_5_Projet_final.ipynb
└── requirements.txt
```

---

##  Astuce

Pour mettre à jour vos dépendances après avoir installé de nouveaux packages :

```bash
pip freeze > requirements.txt
```

---



