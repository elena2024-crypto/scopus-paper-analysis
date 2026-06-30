# scopus-paper-analysis
# Tourism Cluster Analysis - Russian Far East

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/elena2024-crypto/scopus-paper-analysis/blob/main/Scopus_Paper_Analysis_v1.ipynb)

## 📌 Overview
This repository contains the code and data for the research paper analyzing tourism development disparities across 11 federal subjects of the Far Eastern Federal District (FEFD) of Russia.

## 📊 Data
- **Source**: Rosstat (Federal State Statistics Service of Russia), 2023
- **Regions**: 11 federal subjects of the Far Eastern Federal District
- **Indicators**: 10 tourism and service-economic indicators

## 🔬 Methodology
- Z-score standardization for data normalization
- Hierarchical clustering using Ward's method
- K-means clustering for verification
- Block-balanced sensitivity analysis for robustness

## 📈 Key Results
- **3 Clusters identified**:
  - **Leading**: Primorsky Krai, Khabarovsk Krai
  - **Intermediate**: Buryatia, Sakha (Yakutia), Zabaykalsky, Kamchatka, Amur, Sakhalin
  - **Peripheral**: Magadan, Jewish Autonomous Oblast, Chukotka
- **Highest correlations**: r = 0.985, 0.963, 0.900
- **Silhouette scores**: k=2 (0.414), k=3 (0.237)
- **Adjusted Rand Index (Ward vs K-means)**: 1.00

## 📁 Files
- `Scopus_Paper_Analysis_v1.ipynb` - Complete analysis notebook
- `Tourism_Cluster_DFO_2023.xlsx` - Raw data

## 🔧 Requirements
- Python 3.x
- pandas, numpy, matplotlib, scikit-learn, scipy

## 🚀 How to Run
1. Open the notebook in Google Colab
2. Upload the Excel file (`Tourism_Cluster_DFO_2023.xlsx`) to the Colab environment
3. Run all cells (Runtime → Run all)

## 👤 Author
**Hien T. Hoang** - PhD Student, Higher School of Management, RUDN University, Moscow, Russia  
Email: 1042255285@rudn.ru

## 📝 Citation
If you use this code or data, please cite:
> Hoang, H. T., & Bogomolova, E. S. (2026). Tourism Development in the Russian Far East: Spatial Differentiation and Cluster-Based Regional Typology. *Economy of Regions*.

## 📄 License
This project is licensed under the MIT License.
Code, data and results for Scopus manuscript
