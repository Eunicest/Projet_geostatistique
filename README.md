# 🗺️ Analyse Spatiale et Modélisation Géostatistique (Isatis)

## 🎯 Résultats de la modélisation
L'analyse structurale de la "Teneur" a permis de calculer un variogramme expérimental omnidirectionnel. L'ajustement a été réalisé avec un modèle sphérique, donnant les paramètres suivants :
* **Effet de pépite (Nugget) :** 
* **Palier (Sill) :**  *(Rappel : Variance totale = Pépite + Palier)*
* **Portée (Range) :** 

---

## 📝 Contexte et Démarche
Ce projet illustre l'exploration, la caractérisation et la modélisation de la distribution spatiale (X, Y, Z) d'une variable géologique (la "Teneur"). 

La démarche documentée dans ce projet comprend :
* **Analyse Exploratoire (EDA) :** Nettoyage des données, statistiques descriptives et analyse de la distribution.
* **Visualisation Spatiale :** Cartographie 2D pour identifier visuellement la répartition des teneurs.
* **Variographie :** Calcul d'un variogramme expérimental omnidirectionnel avec la bibliothèque `isatis`.
* **Ajustement (Fitting) :** Utilisation d'un modèle sphérique pour quantifier la structure spatiale.

### ⚠️ Limites du projet
Ce travail se concentre uniquement sur l'analyse de la continuité spatiale (variographie) et s'arrête à la validation du modèle d'ajustement. **L'étape d'estimation et d'interpolation spatiale (Krigeage) n'a pas été réalisée dans le cadre de ce notebook.**

### 🛠️ Outils et Technologies
* **Domaines :** Géostatistique, Analyse spatiale
* **Environnement :** Python, Jupyter Notebook
* **Bibliothèques :** `isatis` (module commercial), `pandas`, `numpy`, `matplotlib`, `seaborn`

### 📂 Contenu du dépôt (`Projet_geostatistique`)
* 📓 `analyse_geostatistique.ipynb` : Le notebook contenant la démarche d'analyse et les visualisations.

> 💡 **Note sur la reproductibilité :** La bibliothèque `isatis` dépendant d'une licence commerciale et le jeu de données géologiques n'étant pas public, le code ne peut pas être relancé tel quel. Le notebook est partagé (avec ses sorties pré-calculées) pour illustrer la méthodologie employée.

---
<br>

<details>
<summary>🇬🇧 <b>English version (Click to expand)</b></summary>

## 🎯 Modeling Results
The structural analysis of the "Grade" (Teneur) allowed the computation of an omnidirectional experimental variogram. The fitting was performed using a spherical model, yielding the following parameters:
* **Nugget effect:** 
* **Sill:** 
* **Range:** 

---

## 📝 Context and Workflow
This project illustrates the exploration, characterization, and modeling of the spatial distribution (X, Y, Z) of a geological variable.

The workflow documented in this project includes:
* **Exploratory Data Analysis (EDA):** Data cleaning, descriptive statistics, and distribution analysis.
* **Spatial Visualization:** 2D mapping to visually identify grade distribution.
* **Variography:** Computation of an omnidirectional experimental variogram using the `isatis` library.
* **Fitting:** Using a spherical model to quantify the spatial structure.

### ⚠️ Project Limitations
This work focuses solely on the analysis of spatial continuity (variography) and stops at the validation of the fitted model. **The spatial estimation and interpolation step (Kriging) was not performed in this notebook.**

### 🛠️ Tools & Technologies
* **Domains:** Geostatistics, Spatial Analysis
* **Environment:** Python, Jupyter Notebook
* **Libraries:** `isatis` (commercial module), `pandas`, `numpy`, `matplotlib`, `seaborn`

### 📂 Repository Content (`Projet_geostatistique`)
* 📓 `analyse_geostatistique.ipynb`: The notebook containing the analysis workflow and visualizations.

> 💡 **Reproducibility Note:** Since the `isatis` library requires a commercial license and the geological dataset is not public, the code cannot be re-run as is. The notebook is shared (with pre-computed outputs) to illustrate the methodology used.
</details>