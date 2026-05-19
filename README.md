# Sports Preferences Analysis in Tunisia

**Exploratory data analysis of sports habits and motivations using R**  
EDA · PCA · MCA · Survey Data · FactoMineR · ggplot2

---

## Overview

This project explores sports preferences and habits among individuals in Tunisia. Data was collected through a survey and analyzed using multivariate statistical methods to uncover patterns in sports motivation, behavior, and attitudes.

| | |
|---|---|
| **Data source** | Original survey (Google Forms) |
| **Sample size** | 56 respondents · 47 variables |
| **Language** | R |
| **Methods** | EDA, PCA, MCA |

---

## Methodology

### 1. Data Loading & Overview
- Survey responses imported from CSV
- Dataset: 56 rows × 47 columns (28 categorical, 19 numerical)

### 2. Exploratory Data Analysis (EDA)
- Distribution of sports interest levels
- Univariate analysis of key variables: gender, age, socio-professional category, smoking habits
- Visualization with pie charts, bar plots, histograms

### 3. Principal Component Analysis (PCA)
- Applied to continuous variables: sports pleasure, motivation, environment, mental well-being, stress relief, social aspects, health habits, encouragement
- Dim1 explains **55.7%** of variance, Dim2 explains **10.4%**
- Variables plot and individuals plot with cos² coloring

### 4. Multiple Correspondence Analysis (MCA)
- Applied to categorical variables (columns 43–47): comfort, technicality, aesthetics, price, brand
- Dim1 explains **27.3%**, Dim2 explains **24.8%** (cumulative 52.1% across 2 dimensions)
- Key findings: Comfort is the strongest driver (R² = 0.458, p < 0.001)
- Variable categories map and individuals map

---

## Key Findings

- **Comfort** is the most influential factor in sports equipment choices (R² = 0.458)
- **Technicality** and **aesthetics** are secondary drivers
- PCA reveals a strong primary dimension (55.7%) capturing overall sports engagement
- MCA identifies distinct consumer profiles based on equipment preferences

---

## Tech Stack

```
R
FactoMineR · factoextra · ggplot2 · readr · dplyr
```

---

## Project Structure

```
sports-preferences-analysis/
├── README.md
├── sports_analysis.Rmd     # or .R script
└── data/
    └── survey_responses.csv
```

---

## Getting Started

```r
install.packages(c("FactoMineR", "factoextra", "ggplot2", "readr", "dplyr"))
```

Then open the `.Rmd` file in RStudio and knit to reproduce the analysis.

---

## Author

**Nada Naffeti** — Data Science & AI Engineering Student @ [ESSAI](https://www.essai.tn/)

[LinkedIn](https://linkedin.com/in/nada-naffeti) · [GitHub](https://github.com/Nada-naffeti)
