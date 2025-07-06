# 🦟 Infectious Disease Prediction: Modeling Dengue Incidences in France (2008–2020)

## 📘 Overview

This repository accompanies my Master's thesis, **"Infectious disease prediction: Modeling dengue incidences in France during 2008–2020"**, submitted to the Department of Statistics at the Athens University of Economics and Business.

The **core objective** of this project was to **develop, implement, and compare three predictive models** specifically designed for **forecasting dengue fever outbreaks**, using real-world epidemiological data from France. The goal was to evaluate which model performs best — not only for this specific case, but also in the **broader context of infectious disease forecasting**.

---

## 🎯 Main Goals

- Build and implement three advanced time-series predictive models:
  1. **HHH4 model** (a Generalized Linear Model framework for disease counts)
  2. **KCDE + copulas** (Kernel Conditional Density Estimation)
  3. **Weighted HHH4** (an extension of HHH4 using incidence weighting)

- Apply these models to actual monthly dengue data in France (2008–2020).
- Compare model performance using standard forecasting metrics.
- Discuss implications for **epidemic modeling**, **public health policy**, and **real-time outbreak surveillance**.

---

## ⚗️ Methods and Tools

### 🧠 Core Predictive Models Used

| Model Name            | Description |
|----------------------|-------------|
| **HHH4**             | A GLM-based model designed for infectious disease count data. Captures endemic and epidemic components over time. |
| **KCDE + Copulas**   | A non-parametric, data-driven method for forecasting probabilistic case counts, incorporating copula-based dependencies. |
| **Weighted HHH4**    | An enhanced HHH4 model that incorporates past incidence weighting schemes, improving temporal prediction accuracy. |

All models were developed and evaluated in **R**, with code provided in the `/scripts/` folder.

---

## 🧪 Broader Predictive Modeling Context

This thesis also explores a wide range of **general predictive modeling approaches**, including:

- **Statistical Models**: Linear & logistic regression, GLMs, time-series (ARIMA/SARIMA), Poisson models
- **Machine Learning Models**: Random forests, SVMs, neural networks, gradient boosting
- **Epidemiology-Specific Models**: Compartment models (SIR, SEIR), agent-based models, spatiotemporal and Bayesian frameworks

These were reviewed to understand their theoretical suitability for disease forecasting, especially in outbreak scenarios like dengue fever.

---

## 📊 Results Summary

- **Weighted HHH4** outperformed the other models in predictive accuracy and robustness, especially in capturing the temporal dynamics of dengue outbreaks.
- **KCDE** was useful in estimating distributions but had challenges with sharp trend shifts.
- **Basic HHH4** was solid, but adding incidence weighting improved performance significantly.

These findings reinforce the importance of choosing **domain-specific, well-tuned models** for public health forecasting.

---

## 📂 Project Structure

```text
├── data/                   # Monthly dengue case data (France, 2008–2020)
├── scripts/                # R scripts for model building and forecasting
│   ├── hhh4_model.R
│   ├── kcde_model.R
│   └── weighted_hhh4_model.R
├── results/                # Outputs: forecasts, plots, evaluation metrics
├── thesis.pdf              # Full thesis document (Chatzopoulos_2023)
└── README.md               # Project documentation (this file)

📚 Citation
Chatzopoulos, G. (2023). Infectious disease prediction: Modeling dengue incidences in France during 2008–2020. MSc Thesis, Department of Statistics, Athens University of Economics and Business.
