# 🗺️ Analyse Spatiale et Modélisation Géostatistique (Isatis)

## 🎯 Résultats de la modélisation

L'analyse structurale de la « Teneur » a permis de calculer un variogramme expérimental omnidirectionnel, ajusté avec un modèle sphérique :

| Paramètre | Valeur | Unité |
| :--- | :---: | :---: |
| Effet de pépite (nugget) | 0,001783 | (unité de la teneur)² |
| Palier partiel (partial sill) | 0,002470 | (unité de la teneur)² |
| Palier total (pépite + palier partiel) | 0,004253 | (unité de la teneur)² |
| Portée (range) | 1721,57 | m |

*Les coordonnées de travail sont en mètres. L'unité de la teneur n'est pas précisée dans les données fournies.*

**Interprétation :**
- La pépite représente environ **42 %** de la variance totale : la dépendance spatiale est modérée, avec une part importante de variabilité à très courte distance ou de bruit de mesure.
- Au-delà de **1721,57 m**, le modèle considère que deux mesures ne sont plus corrélées.

---

## 📝 Contexte et démarche

Exploration, caractérisation et modélisation de la distribution spatiale (X, Y, Z) d'une variable géologique, la « Teneur ».

Grille de travail : 60 × 60 × 75 nœuds, mailles de 33,33 m × 33,33 m × 2 m (environ 2 000 m × 2 000 m × 150 m).

- **Analyse exploratoire (EDA) :** nettoyage des données, statistiques descriptives, analyse de la distribution.
- **Visualisation spatiale :** cartographie 2D pour repérer visuellement la répartition des teneurs.
- **Variographie :** calcul d'un variogramme expérimental omnidirectionnel avec la bibliothèque `isatis`.
- **Ajustement :** modèle sphérique pour quantifier la structure spatiale.

### ⚠️ Limites du projet
- Le travail s'arrête à l'analyse de la continuité spatiale (variographie) : **le krigeage (estimation et interpolation spatiale) n'a pas été réalisé** dans ce notebook.
- Seul un variogramme **omnidirectionnel** a été calculé : l'anisotropie n'a pas été étudiée.
- La portée (1721,57 m) est du même ordre de grandeur que l'étendue de la grille (environ 2 000 m) : le palier est probablement peu contraint par les données .
- Le code ne peut pas être relancé tel quel (voir la note de reproductibilité).

### 🛠️ Outils et technologies
- **Domaines :** géostatistique, analyse spatiale
- **Environnement :** Python, Jupyter Notebook
- **Bibliothèques :** `isatis` (module commercial), `pandas`, `numpy`, `matplotlib`, `seaborn`

### 📂 Contenu du dépôt
- 📓 `analyse_geostatistique.ipynb` : notebook contenant la démarche d'analyse et les visualisations.

> 💡 **Reproductibilité :** la bibliothèque `isatis` dépend d'une licence commerciale et le jeu de données géologiques n'est pas public. Le code ne peut donc pas être relancé tel quel ; le notebook est partagé avec ses sorties pré-calculées pour illustrer la méthodologie.

**Pistes d'amélioration :** réaliser le krigeage et sa validation croisée, tester des variogrammes directionnels

---

<details>
<summary>🇬🇧 <b>English version</b></summary>

# 🗺️ Spatial Analysis and Geostatistical Modeling (Isatis)

## 🎯 Modeling results

The structural analysis of the grade ("Teneur") produced an omnidirectional experimental variogram, fitted with a spherical model:

| Parameter | Value | Unit |
| :--- | :---: | :---: |
| Nugget effect | 0.001783 | (grade unit)² |
| Partial sill | 0.002470 | (grade unit)² |
| Total sill (nugget + partial sill) | 0.004253 | (grade unit)² |
| Range | 1721.57 | m |

*Working coordinates are in meters. The unit of the grade is not specified in the data provided.*

**Interpretation:**
- The nugget represents about **42%** of the total variance: spatial dependence is moderate, with a substantial share of very short-distance variability or measurement noise.
- Beyond **1721.57 m**, the model considers two measurements as uncorrelated.

## 📝 Context and workflow

Exploration, characterization and modeling of the spatial distribution (X, Y, Z) of a geological variable, the grade.

Working grid: 60 × 60 × 75 nodes, mesh size 33.33 m × 33.33 m × 2 m (about 2,000 m × 2,000 m × 150 m).

- **Exploratory data analysis:** cleaning, descriptive statistics, distribution analysis.
- **Spatial visualization:** 2D mapping to visually identify grade distribution.
- **Variography:** omnidirectional experimental variogram with the `isatis` library.
- **Fitting:** spherical model to quantify spatial structure.

### ⚠️ Limitations
- The work stops at spatial continuity analysis (variography): **kriging (spatial estimation and interpolation) was not performed** in this notebook.
- Only an **omnidirectional** variogram was computed: anisotropy was not studied.
- The range (1721.57 m) is of the same order as the grid extent (about 2,000 m): the sill is probably poorly constrained by the data 
- The code cannot be re-run as is (see reproducibility note).

### 🛠️ Tools
- **Domains:** geostatistics, spatial analysis
- **Environment:** Python, Jupyter Notebook
- **Libraries:** `isatis` (commercial module), `pandas`, `numpy`, `matplotlib`, `seaborn`

### 📂 Repository content
- 📓 `analyse_geostatistique.ipynb`: notebook with the analysis workflow and visualizations.

> 💡 **Reproducibility:** `isatis` requires a commercial license and the geological dataset is not public, so the code cannot be re-run as is. The notebook is shared with pre-computed outputs to illustrate the methodology.

**Possible improvements:** perform kriging and cross-validation, test directional variograms.

</details>
