# Tourism Development in the Russian Far East: Spatial Differentiation and Cluster-Based Regional Typology

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/elena2024-crypto/scopus-paper-analysis/blob/main/Tourism_Cluster_DFE_2023_Analysis%20Final.ipynb)

**Python** | **License** | **Open In Colab**

This repository contains the data, code, and results for the research paper:

> Hoang, H. T., & Bogomolova, E. S. (2026). Tourism Development in the Russian Far East: Spatial Differentiation and Cluster-Based Regional Typology. *Economy of Regions*.

---

## 📋 Abstract

The Russian Far East is one of the largest and most spatially heterogeneous macroregions of the Russian Federation. Despite substantial natural, cultural and recreational resources, tourism development across its constituent regions remains highly uneven. This study aims to identify spatial patterns of tourism development in the Far Eastern Federal District and construct a cluster-based typology using official statistical data for 2023.

**Key findings reveal three distinct clusters:**

| Cluster | Regions |
|:---|:---|
| **Leading Cluster** (2 regions) | Primorsky Krai, Khabarovsk Krai |
| **Intermediate Cluster** (6 regions) | Buryatia, Sakha (Yakutia), Zabaykalsky Krai, Kamchatka Krai, Amur Oblast, Sakhalin Oblast |
| **Peripheral Cluster** (3 regions) | Magadan Oblast, Jewish Autonomous Oblast, Chukotka Autonomous Okrug |

---

## 📊 Data Source

The empirical analysis uses cross-sectional data for 2023 from the official statistical handbook:

> Rosstat. (2024). *Regions of Russia. Socio-economic indicators. 2024*. Moscow: Federal State Statistics Service.

**Dataset characteristics:**
- **Observations:** 11 federal subjects of the Far Eastern Federal District
- **Indicators:** 10 tourism and service-economic indicators
- **Dimensions:** Tourism infrastructure, tourist flows, business activity, cultural participation, service-economic environment

---

## 🔬 Methodology

The analysis follows a three-stage framework:

| Stage | Method | Purpose |
|:---|:---|:---|
| 1 | Z-score standardization | Ensure cross-indicator comparability |
| 2 | Hierarchical clustering (Ward's method) | Identify natural groupings and visualize similarity structure |
| 3 | K-means clustering | Verify stability of regional groupings |

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
|:---|:---|:---|:---|
| 2 | 0.414 | 8.29 | 0.752 |
| **3** | **0.237** | **7.12** | **1.095** |
| 4 | 0.231 | 6.66 | 0.770 |
| 5 | 0.160 | 6.57 | 0.608 |

*Note: The three-cluster solution was selected due to superior interpretability and policy relevance.*

### Cluster Characteristics

| Indicator | Leading Cluster | Intermediate Cluster | Peripheral Cluster |
|:---|:---|:---|:---|
| Collective accommodation establishments (units) | 427.50 | 226.00 | 27.00 |
| Tourists accommodated (thousand persons) | 965.00 | 334.67 | 59.67 |
| Tourism enterprises (units) | 115.50 | 59.67 | 5.00 |
| Tour packages sold (thousand units) | 38.65 | 11.58 | 0.82 |
| Retail trade turnover (million RUB) | 556,725.00 | 240,626.33 | 33,695.00 |
| Paid services (million RUB) | 185,694.00 | 65,860.17 | 10,880.33 |

---

## 📊 Figures

### Figure 1. Hierarchical Dendrogram

The dendrogram shows the similarity structure among the 11 regions based on Ward's hierarchical clustering.

![Figure 1. Dendrogram](https://github.com/elena2024-crypto/scopus-paper-analysis/blob/main/Figure1_Dendrogram%20(1).png)

### Figure 2. Spatial Distribution of Tourism Clusters

The map shows the geographical distribution of the three tourism-development clusters across the Far Eastern Federal District.

![Figure 2. Cluster Map](https://github.com/elena2024-crypto/scopus-paper-analysis/blob/main/Figure_2_Tourism_Clusters.png)

### Figure 3. Cluster Profiles

Standardized profiles of the three tourism-development clusters across 10 indicators (z-scores).

![Figure 3. Cluster Profiles](https://github.com/elena2024-crypto/scopus-paper-analysis/blob/main/Figure3_Cluster_Profile%20(1).png)

---

## 📁 Repository Structure
