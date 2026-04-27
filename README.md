# Chicago Crime Detection

**CMPE 255 – Data Mining | Spring 2026 | Group 9**

Predicting arrest outcomes and identifying crime hotspots in Chicago using machine learning on the City of Chicago open crime dataset.

## Team

| GitHub    | Role                       |
| --------- | -------------------------- |
| @Lorelei  | Data Collection & Cleaning |
| @cahide   | EDA & Visualization        |
| @SajaA    | Statistical Analysis       |
| @Scottch7 | Modeling & Quality         |

**Instructor:** Prof. Bertin Cordova-Diba

## Project Overview

- **Primary task:** Binary classification — predict whether a crime incident results in an arrest
- **Secondary task:** Forecast crime counts by area and time period
- **Methods:** Logistic Regression (baseline), Decision Trees, Random Forest, XGBoost, DBSCAN clustering for spatial features
- **Class imbalance handling:** SMOTE and class weighting
- **Evaluation:** Accuracy, Precision, Recall, F1-score, ROC-AUC, confusion matrix

## Dataset

- **Source:** [City of Chicago Open Data Portal](https://data.cityofchicago.org/Public-Safety/Crimes-2001-to-Present/ijzp-q8t2)
- **API:** Socrata Open Data API (SODA)
- **Size:** 8.5M+ records (2001–present), 22 columns
- **Updated:** Daily

## Repository Structure

```
.
├── README.md
├── notebooks/
│   └── check_in_1_chicago_crime_eda.ipynb     # Initial EDA — Check-in 1
└── figures/
    └── check_in_1/                            # Plots generated during Check-in 1 EDA
```

## Getting Started

### Requirements

- Python 3.10+
- `pandas`, `matplotlib`, `seaborn`, `requests`

```bash
pip install pandas matplotlib seaborn requests
```

### Run the EDA Notebook

```bash
jupyter notebook notebooks/check_in_1_chicago_crime_eda.ipynb
```

The notebook pulls a 50,000-row sample from the SODA API and uses server-side aggregation for full-dataset trend analysis (no large local downloads required).

## Status

- [x] Project proposal submitted
- [x] Dataset identified and explored (Check-in 1)
- [x] GitHub repository created
- [ ] Feature engineering and preprocessing
- [ ] Model training and evaluation
- [ ] Final report
