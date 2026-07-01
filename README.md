# Tourism Development in the Russian Far East: Spatial Differentiation and Cluster-Based Regional Typology

[![Python](https://img.shields.io/badge/Python-3.10+-3776AB?logo=python&logoColor=white)](https://www.python.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/elena2024-crypto/tourism-russian-far-east/blob/main/Scopus_Paper_Analysis_v1.ipynb)

**This repository contains the data, code, and results for the research paper:**

> **Hoang, H. T., & Bogomolova, E. S.** (2026). Tourism Development in the Russian Far East: Spatial Differentiation and Cluster-Based Regional Typology. *Economy of Regions*.

---

## 📋 Abstract

The Russian Far East is one of the largest and most spatially heterogeneous macroregions of the Russian Federation. Despite substantial natural, cultural and recreational resources, tourism development across its constituent regions remains highly uneven. This study aims to identify spatial patterns of tourism development in the Far Eastern Federal District and construct a cluster-based typology using official statistical data for 2023.

**Key findings** reveal three distinct clusters:
- **Leading Cluster** (2 regions): Primorsky Krai, Khabarovsk Krai
- **Intermediate Cluster** (6 regions): Buryatia, Sakha (Yakutia), Zabaykalsky Krai, Kamchatka Krai, Amur Oblast, Sakhalin Oblast
- **Peripheral Cluster** (3 regions): Magadan Oblast, Jewish Autonomous Oblast, Chukotka Autonomous Okrug

---

## 📊 Data Source

The empirical analysis uses cross-sectional data for 2023 from the official statistical handbook:

> **Rosstat.** (2024). *Regions of Russia. Socio-economic indicators. 2024*. Moscow: Federal State Statistics Service.

**Dataset characteristics:**
- **Observations:** 11 federal subjects of the Far Eastern Federal District
- **Indicators:** 10 tourism and service-economic indicators
- **Dimensions:** Tourism infrastructure, tourist flows, business activity, cultural participation, service-economic environment

---

## 🔬 Methodology

The analysis follows a three-stage framework:

| Stage | Method | Purpose |
| :--- | :--- | :--- |
| **1** | Z-score standardization | Ensure cross-indicator comparability |
| **2** | Hierarchical clustering (Ward's method) | Identify natural groupings and visualize similarity structure |
| **3** | K-means clustering | Verify stability of regional groupings |

**Validation techniques:**
- Silhouette coefficient
- Calinski-Harabasz index
- Davies-Bouldin index
- Adjusted Rand Index (ARI) between Ward and K-means classifications
- One-way ANOVA with Tukey HSD post-hoc tests
- Sensitivity analysis (leave-one-out and block-balanced specifications)

**Software:**
- Python 3.10+ (pandas, NumPy, SciPy, scikit-learn)
- QGIS 4.0.3 for spatial visualization

---

## 📈 Key Results

### Cluster Validation Metrics

| Number of Clusters (k) | Silhouette Score | Calinski-Harabasz Index | Davies-Bouldin Index |
| :---: | :---: | :---: | :---: |
| 2 | 0.414 | 8.29 | 0.752 |
| **3** | **0.237** | **7.12** | **1.095** |
| 4 | 0.231 | 6.66 | 0.770 |
| 5 | 0.160 | 6.57 | 0.608 |

*Note: The three-cluster solution was selected due to superior interpretability and policy relevance.*

### Cluster Characteristics

| Indicator | Leading Cluster | Intermediate Cluster | Peripheral Cluster |
| :--- | :---: | :---: | :---: |
| Collective accommodation establishments (units) | 427.50 | 226.00 | 27.00 |
| Tourists accommodated (thousand persons) | 965.00 | 334.67 | 59.67 |
| Tourism enterprises (units) | 115.50 | 59.67 | 5.00 |
| Tour packages sold (thousand units) | 38.65 | 11.58 | 0.82 |
| Retail trade turnover (million RUB) | 556,725.00 | 240,626.33 | 33,695.00 |
| Paid services (million RUB) | 185,694.00 | 65,860.17 | 10,880.33 |

### Spatial Distribution

The leading cluster is concentrated in the southern Pacific part of the macroregion. The intermediate cluster is geographically extensive and internally diverse, while the peripheral cluster is spatially discontinuous.

---
## 🗺️ Spatial Distribution of Tourism Clusters

[Cluster Map](results/figures/cluster_map.png)](https://github.com/elena2024-crypto/scopus-paper-analysis/blob/main/Figure_2_Tourism_Clusters.png)

*Figure 2. Spatial distribution of tourism-development clusters in the Far Eastern Federal District.*

---

## 📁 Repository Structure

