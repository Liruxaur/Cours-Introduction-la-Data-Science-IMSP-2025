# Travaux Pratiques — Deep Learning

Ce dossier contient un ensemble de **TP (Travaux Pratiques)** destinés à accompagner le cours de Deep Learning.

Les notebooks couvrent notamment :
- Tenseurs et gradients
- Réseaux neuronaux (fondations)
- PyTorch (training / inference / GPU)
- CNN, RNN, GRU
- Visualisation des données et de l’apprentissage

---

## ⚙️ Installation

Il est **fortement recommandé** d’utiliser un environnement virtuel.

### 1. Créer un environnement virtuel

```bash
python -m venv venv
source venv/bin/activate      # Linux / Mac
# ou
venv\Scripts\activate         # Windows
```

---

### 2. Installer les dépendances

```bash
pip install -r requirements.txt
```

---

## 🚀 Lancer les notebooks

```bash
jupyter notebook
```

Puis ouvrir le notebook souhaité.

---

## 💻 GPU (optionnel)

Si vous avez un GPU NVIDIA compatible CUDA, vérifiez dans Python :

```python
import torch
print(torch.cuda.is_available())
```

---

## 📌 Recommandations

- Utiliser **Python 3.9 – 3.11**
- Ne pas mélanger plusieurs environnements Python
- En cas d’erreur, recréer l’environnement proprement
- Bien lire les consignes dans chaque notebook

---

## 👨‍🏫 Objectif pédagogique

Ces TP visent à :
- Comprendre les mécanismes du Deep Learning
- Manipuler PyTorch correctement
- Visualiser ce que fait un modèle
- Passer du théorique au pratique

---

Bon TP 🚀
