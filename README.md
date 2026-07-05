# 🏙️ São Paulo Rent Price Prediction

Machine Learning project developed as part of a postgraduate program in Data Science.

The objective is to predict the average rental price (R$/m²) of neighborhoods in São Paulo using demographic and geographic characteristics and identify neighborhood profiles through clustering.

---

## Project Overview

This project combines multiple public datasets to investigate whether demographic characteristics can explain rental prices across São Paulo neighborhoods.

Two complementary approaches were developed:

- **Regression:** predict the average rental price per square meter.
- **Clustering:** identify groups of neighborhoods with similar demographic characteristics.

---

## Dataset

Public datasets were integrated from multiple sources:

- FIPEZAP
- IBGE
- Banco Central
- Other public demographic datasets

The datasets are **not included** in this repository.

Instructions to reproduce the dataset are available under `data/raw/`.

---

## Machine Learning Pipeline

```
Data Collection
        ↓
Data Cleaning
        ↓
Feature Engineering
        ↓
Exploratory Data Analysis
        ↓
Regression Models
        ↓
Temporal Validation
        ↓
Hyperparameter Tuning
        ↓
Model Evaluation
        ↓
Neighborhood Clustering
```

---

## Models

Regression

- Dummy Regressor (Baseline)
- Linear Regression
- Ridge Regression
- LightGBM

Clustering

- K-Means
- Agglomerative Clustering

---

## Results

| Metric | Best Model |
|---------|-----------:|
| MAE | **2.93** |
| RMSE | **3.34** |
| R² | **0.964** |

Main findings:

- Demographic variables are strong predictors of rental prices.
- LightGBM achieved the best predictive performance.
- K-Means generated clusters consistent with the existing neighborhood tiers.

---

## Repository structure

```
notebooks/
    Main notebook

reports/
    Executive summary

data/
    Instructions to obtain the datasets

images/
    Figures used in the README
```

---

## Technologies

- Python
- Pandas
- NumPy
- Scikit-Learn
- LightGBM
- Matplotlib

---

## Future work

- Incorporate additional geographic variables.
- Increase neighborhood coverage.
- Evaluate feature importance (e.g. SHAP).
- Automate the data pipeline.

---

## License

MIT License
