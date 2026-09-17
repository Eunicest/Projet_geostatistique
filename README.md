# 🗺️ Analyse Spatiale et Modélisation Géostatistique avec Isatis
*Spatial Analysis and Geostatistical Modeling using Isatis*

🌍 **[English version below](#english-version)**

---

## 🇫🇷 Version Française

### 📝 Contexte et Objectif
Ce projet a été mené afin d'explorer, caractériser et modéliser la distribution tridimensionnelle (X, Y, Z) d'une variable géologique (la "Teneur"). 
L'objectif principal est de quantifier la continuité et la dépendance spatiale de ces données en utilisant des outils géostatistiques avancés. 

La démarche documentée dans ce projet comprend :
* **L'Analyse Exploratoire des Données (EDA) :** Nettoyage des données, statistiques descriptives et analyse de la distribution (histogrammes, boîtes à moustaches).
* **La Visualisation Spatiale :** Cartographie 2D (scatter plots) pour identifier visuellement les zones de forte ou faible concentration.
* **La Géostatistique :** Calcul d'un variogramme expérimental omnidirectionnel.
* **La Modélisation :** Ajustement (fitting) du variogramme expérimental à l'aide d'un modèle mathématique (modèle sphérique) pour évaluer la variance spatiale et l'effet de pépite.

### 🛠️ Outils et Technologies
* **Langage & Environnement :** Python, Jupyter Notebook
* **Domaines d'application :** Géostatistique, Analyse spatiale, Ingénierie des données
* **Bibliothèques principales :** `isatis` (GeoStats), `pandas`, `numpy`, `matplotlib`, `seaborn`

### 📂 Contenu du dépôt (`Peojet_geostatistique`)
* `Projet_Eunice (3).ipynb` : Le notebook Jupyter principal illustrant l'ensemble de la démarche d'analyse de données, les calculs géostatistiques et les visualisations associées.

> ⚠️ **Note de traçabilité :** Le jeu de données original (contenant les coordonnées spatiales et les teneurs) n'est pas inclus dans ce dépôt. Ce notebook est partagé en tant que portfolio pour documenter la méthode d'analyse, l'approche algorithmique et la maîtrise de la bibliothèque Isatis.

---
<br>

<a name="english-version"></a>
## 🇬🇧 English Version

### 📝 Context and Objective
This project was conducted to explore, characterize, and model the three-dimensional (X, Y, Z) distribution of a geological variable (the "Grade" or "Teneur"). 
The main objective is to quantify the spatial continuity and dependence of this data using advanced geostatistical tools.

The workflow documented in this project includes:
* **Exploratory Data Analysis (EDA):** Data cleaning, descriptive statistics, and distribution analysis (histograms, boxplots).
* **Spatial Visualization:** 2D mapping (scatter plots) to visually identify areas of high or low concentration.
* **Geostatistics:** Computation of an omnidirectional experimental variogram.
* **Modeling:** Fitting the experimental variogram using a mathematical model (spherical model) to assess spatial variance and the nugget effect.

### 🛠️ Tools & Technologies
* **Language & Environment:** Python, Jupyter Notebook
* **Application Domains:** Geostatistics, Spatial Analysis, Data Engineering
* **Core Libraries:** `isatis` (GeoStats), `pandas`, `numpy`, `matplotlib`, `seaborn`

### 📂 Repository Content (`Peojet_geostatistique`)
* `Projet_Eunice (3).ipynb`: The main Jupyter notebook illustrating the entire data analysis workflow, geostatistical calculations, and associated visualizations.

> ⚠️ **Traceability Note:** The original dataset (containing spatial coordinates and grades) is not included in this repository. This notebook is shared as a portfolio piece to document the analytical method, algorithmic approach, and proficiency with the Isatis library.
