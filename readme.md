# Analyse des données

## Description

Ce projet concerne l'analyse des données issues d'un processus industriel. Les données couvrent plusieurs étapes de production, incluant les conditions ambiantes de l'usine, les propriétés des matières premières, les variables de processus de différentes machines, et les mesures de sortie principales et secondaires à contrôler.

## Contributeurs

- Amine LADEL
- Thomas JEANDENANT
- Toinot GURY

## Méthodes et Logique

Le projet inclut plusieurs étapes d'analyse et de traitement des données. Voici un aperçu des principales étapes et des bibliothèques utilisées :

### Importation des Bibliothèques

```python
# Importation des bibliothèques nécessaires
import pandas as pd
import numpy as np
from matplotlib import pyplot as plt
import seaborn as sns
from plotly import express as px
from plotly import graph_objects as go
import warnings

# Configuration initiale
warnings.filterwarnings("ignore")
sns.set()
# %matplotlib inline
```

### Chargement des Données

```python
# Charger les données
df = pd.read_csv("continuous_factory_process.csv")

# Afficher les premières lignes
df.head()
```

## Structure des Données

Les données sont organisées comme suit :

- Horodatage
- Conditions ambiantes de l'usine
- Première étape : propriétés des matières premières et variables de processus pour les Machines 1, 2 et 3
- Paramètres du processus du combinateur
- Sortie principale à contrôler : mesures de 15 caractéristiques avec consigne ou cible pour chacune
- Deuxième étape : variables de processus pour les Machines 4 et 5
- Sortie secondaire à contrôler : mesures de 15 caractéristiques avec consigne ou cible pour chacune

## Instructions pour exécuter le projet

1. Assurez-vous d'avoir installé les bibliothèques nécessaires : pandas, numpy, matplotlib, seaborn, plotly.
2. Clonez le dépôt du projet et placez-vous dans le répertoire correspondant.
3. Exécutez le notebook Jupyter pour reproduire l'analyse des données.
