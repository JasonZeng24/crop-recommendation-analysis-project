# 🌾 Crop Recommendation Analysis

A machine learning project that analyzes agricultural sensor data to recommend optimal crops and identify key environmental factors affecting crop growth.

## 📊 Project Overview

This project explores the [Crop Recommendation Dataset](https://www.kaggle.com/datasets/atharvaingle/crop-recommendation-dataset) to understand how environmental conditions — including soil nutrients, temperature, humidity, pH, and rainfall — influence crop selection. The analysis includes exploratory data analysis (EDA), feature importance analysis, and a Random Forest classification model.

## 🔍 Key Findings

- **Rainfall** and **humidity** are the most influential factors in crop recommendation (importance scores: 0.227 and 0.211)
- **Potassium (K)** and **Phosphorus (P)** are the most important soil nutrients
- Random Forest classifier achieves **99.32% accuracy** across 22 crop types

## 🛠️ Tech Stack

| Component | Technology |
|-----------|------------|
| Language | Python 3.8+ |
| Data Analysis | pandas, NumPy |
| Visualization | matplotlib, seaborn |
| ML Model | scikit-learn (Random Forest) |
| Environment | Jupyter Notebook |

## 📁 Project Structure

```
crop-recommendation-analysis-project/
└── agri-prediction-poc/
    ├── data/
    │   └── Crop_recommendation.csv
    └── notebooks/
        └── 01_data_exploration.ipynb
```

## 📈 Analysis Pipeline

1. **Data Exploration** — Load dataset (2200 samples, 8 features, 22 crop labels), check for missing values, compute summary statistics
2. **Filtering & EDA** — Identify high-rainfall crops, analyze extreme weather conditions, visualize average rainfall by crop
3. **Feature Engineering** — Create binary features (e.g., `is_hot`), compute correlation heatmap across all features
4. **GroupBy Analysis** — Summarize mean environmental conditions per crop type
5. **Model Training** — Train Random Forest classifier with 80/20 train-test split
6. **Feature Importance** — Visualize which factors matter most for crop prediction

## 🚀 Getting Started

```bash
git clone https://github.com/JasonZeng24/crop-recommendation-analysis-project.git
cd crop-recommendation-analysis-project
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
jupyter notebook
```

## 📊 Model Performance

| Metric | Score |
|--------|-------|
| Accuracy | 99.32% |
| Top Feature | Rainfall (0.227) |
| 2nd Feature | Humidity (0.211) |
| Classes | 22 crop types |

## 👤 Author

**Jason Zeng (Jun-Wei Zeng)**
- GitHub: [@JasonZeng24](https://github.com/JasonZeng24)
