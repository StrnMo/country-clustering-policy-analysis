# 🌍 Country Development Clustering and Budget Allocation Analysis

A comprehensive data science project analyzing **167 countries** using **9 development indicators** to identify socioeconomic profiles and inform an illustrative **$1 billion budget allocation** strategy.

---

## 📊 Project Overview

This project combines **Exploratory Data Analysis (EDA)** with **K-Means clustering** to uncover meaningful country groupings based on health, economic, and social indicators. The analysis identifies **5 distinct development profiles** and demonstrates how clustering insights can inform resource allocation decisions.

### Key Results

| Metric | Result |
|:---|:---|
| Countries Analyzed | 167 |
| Development Indicators | 9 |
| Identified Clusters | 5 |
| Most Vulnerable Profile | 44 countries (26.3%) |
| Most Advanced Profile | 31 countries (18.6%) |
| Illustrative Budget | $1,000,000,000 |
| Largest Allocation | 45% ($450M) to High Development Vulnerability |
| PCA Variance Explained | 71.6% |

---

## 📁 Repository Structure

```
country-clustering-analysis/
│
├── data/
│   ├── raw/
│   │   └── Country-data.csv
│   └── processed/
│       ├── countries_transformed_scaled.csv
│       ├── countries_clustered_final.csv
│       ├── cluster_profiles.csv
│       ├── cluster_geographic_data.csv
│       ├── budget_allocation_final.csv
│       ├── yeojohnson_transformer.pkl
│       ├── standard_scaler.pkl
│       └── (23+ additional CSV files)
│
├── notebooks/
│   ├── 01_eda_analysis.ipynb
│   ├── 02_clustering_analysis.ipynb
│   └── 03_Report.ipynb
│
├── figures/
│   ├── eda/
│   │   ├── before_after_transformation.png
│   │   ├── correlation_matrix.png
│   │   ├── key_variable_distributions.png
│   │   ├── multivariate_outliers_log.png
│   │   ├── outlier_boxplots.png
│   │   ├── outlier_countries_heatmap.png
│   │   ├── skewness_kurtosis.png
│   │   └── transformation_improvement_chart.png
│   │
│   └── clustering/
│       ├── pca_clusters_professional.png
│       ├── cluster_profiles_heatmap.png
│       ├── radar_charts_combined.png
│       ├── parallel_coordinates.png
│       ├── elbow_curve.png
│       ├── k5_selection_justification.png
│       ├── cluster_sizes.png
│       ├── world_map_clusters.png
│       ├── sankey_budget.png
│       ├── budget_allocation_final.png
│       ├── cluster_analysis_dashboard.png
│       └── (15+ additional PNG/HTML files)
│
├── reports/
│   ├── final/
│   │   └── Report.pdf
│   └── drafts/
│
├── tables/
│   ├── cluster_centroids.csv
│   ├── cluster_summary_stats.csv
│   ├── countries_by_cluster.csv
│   └── normalized_means.csv
│
├── .venv/
├── requirements.txt
├── README.md
└── .gitignore
```

---

## 🚀 Getting Started

### Prerequisites

- Python 3.9 or higher
- pip package manager

### Installation

```bash
# 1. Clone the repository
git clone https://github.com/strnMo/country-clustering-analysis.git
cd country-clustering-analysis

# 2. Create and activate virtual environment
python -m venv .venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate

# 3. Install dependencies
pip install -r requirements.txt
```

### Run the Analysis

```bash
# 4. Launch Jupyter Notebook
jupyter notebook

# 5. Run notebooks in order
#    - notebooks/01_eda_analysis.ipynb
#    - notebooks/02_clustering_analysis.ipynb
#    - notebooks/03_Report.ipynb
```

---

## 📊 Key Findings

### Data Quality

| Check | Result |
|:---|:---|
| Missing Values | ✅ 0 (0%) |
| Duplicate Rows | ✅ 0 |
| Complete Observations | ✅ 167 (100%) |

### Transformation Impact

| Metric | Before | After | Improvement |
|:---|:---|:---|:---|
| Average Skewness | 2.23 | 0.08 | **96.4%** |
| Maximum Skewness | 5.15 | 0.18 | **96.5%** |

### Five Development Profiles

| Cluster | Profile | Countries | Priority | Budget |
|:---|:---|:---|:---|:---|
| 0 | Intermediate Development | 41 | High | 25% (\$250M) |
| 1 | High Development | 31 | Very Low | 2% (\$20M) |
| 2 | High Development Vulnerability | 44 | Very High | 45% (\$450M) |
| 3 | Trade-Intensive Development | 27 | Medium | 8% (\$80M) |
| 4 | Higher-Inflation Development | 24 | High | 20% (\$200M) |

---

## 📖 Full Report

A comprehensive **25-page PDF report** is available:

[![Download PDF](https://img.shields.io/badge/📥-Download%20Report-red?style=for-the-badge&logo=adobeacrobatreader)](reports/final/Report.pdf)

| Format | Link |
|:---|:---|
| **PDF Report** | [📥 Download PDF](reports/final/Report.pdf) |
| **Jupyter Notebook** | [📓 View Notebook](notebooks/03_Report.ipynb) |

> **Note:** PDF files cannot be previewed directly on GitHub. Please download the file to view it.

---

## 🛠️ Dependencies

```txt
# Core Data Manipulation
pandas>=1.3.0
numpy>=1.21.0

# Visualization
matplotlib>=3.4.0
seaborn>=0.11.0
plotly>=5.0.0
kaleido>=1.0.0

# Machine Learning & Statistics
scikit-learn>=1.0.0
scipy>=1.7.0

# Jupyter Notebook
jupyter>=1.0.0
nbconvert>=6.0.0
ipykernel>=6.0.0

# Utilities
joblib>=1.1.0
openpyxl>=3.0.0
tqdm>=4.62.0
```

---

## 📁 Data Files Overview

### Processed Data (`data/processed/`)

| File | Description |
|:---|:---|
| `countries_transformed_scaled.csv` | Final preprocessed data (scaled & transformed) |
| `countries_clustered_final.csv` | Data with cluster assignments |
| `cluster_profiles.csv` | Mean values per cluster |
| `cluster_geographic_data.csv` | Geographic mapping data |
| `budget_allocation_final.csv` | Budget allocation results |
| `yeojohnson_transformer.pkl` | Saved transformer model |
| `standard_scaler.pkl` | Saved scaler model |

---

## 👤 Author

  
- Email:  mo110.st77@gmail.com  
- GitHub: https://github.com/StrnMo

---

## 📊 Quick Reference

| Metric | Value |
|:---|:---|
| Countries | 167 |
| Features | 9 |
| Clusters | 5 |
| Silhouette Score | 0.2226 |
| PCA Variance | 71.6% |
| Budget | $1B |
| Report Pages | 25 |
| EDA Figures | 8 |
| Clustering Figures | 27+ |

---

**Last Updated:** August 2026