# Explainable AI for Strategic Decision-Making in SMEs

Master's Thesis — M.Sc. Big Data and Business Analytics  
FOM University of Applied Sciences, Essen, Germany  
Grade: 1.9 | October 2025 – February 2026

---

## Overview

Black-box machine learning models are powerful but insufficient for high-stakes enterprise environments where decision-makers need to understand why a model recommends what it does before acting on it. This thesis designs, implements, and validates a full explainable AI (XAI) framework for strategic decision support in enterprise contexts.

The framework integrates multi-source heterogeneous data with SHAP and LIME interpretability tools, bridging the gap between predictive performance and human-understandable reasoning.

Research question: How can explainable AI be systematically integrated into enterprise decision pipelines to achieve both high predictive accuracy and full model transparency?

---

## Models and Performance

| Model | Accuracy | ROC AUC | Notes |
|---|---|---|---|
| XGBoost | Best performer | Superior | Primary model |
| Random Forest | Baseline | Competitive | Comparison model |

---

## XAI Methods Applied

| Method | Type | Purpose |
|---|---|---|
| SHAP TreeExplainer | Global + Local | Feature ranking, case-level explanation |
| SHAP SummaryPlot | Global | Visual feature importance across dataset |
| LIME | Local | Individual prediction explanation for stakeholders |

---

## Framework Architecture

```
Data Layer
Multi-source heterogeneous enterprise data

Preprocessing Layer
Cleaning, encoding, scaling, feature selection

Model Layer
XGBoost and Random Forest with cross-validation

Explainability Layer
SHAP (global rankings, dependence plots, interaction effects)
LIME (local case-level explanations, feature weights)

Decision Support Layer
Human-readable outputs for non-technical stakeholders
Audit trails and compliance-ready documentation
```

---

## Key Findings

- XGBoost outperformed Random Forest in predictive accuracy across all tested decision contexts
- SHAP provided stable global explanations with consistent feature rankings across data splits
- LIME excelled at local explanations, enabling case-by-case justification for individual predictions
- Interpretability did not significantly reduce accuracy versus black-box baselines
- Administrative and contextual variables frequently ranked among top predictors

---

## Tech Stack

| Category | Tools |
|---|---|
| Language | Python 3.12 |
| ML Models | XGBoost, Random Forest (Scikit-learn) |
| Explainability | SHAP, LIME |
| Data Processing | Pandas, NumPy |
| Visualisation | Matplotlib, Seaborn |
| Environment | Jupyter Notebook |

---

## Repository Structure

```
msc-thesis-xai-decision-making/
|
|-- thesis_xai_framework.ipynb
|-- README.md
```

---

## How to Run

```bash
git clone https://github.com/Anurag101723/msc-thesis-xai-decision-making.git
cd msc-thesis-xai-decision-making
pip install pandas numpy scikit-learn xgboost shap lime matplotlib seaborn
jupyter notebook thesis_xai_framework.ipynb
```

---

## Academic Context

Program: M.Sc. Big Data and Business Analytics  
Institution: FOM University of Applied Sciences, Essen, Germany  
Period: October 2025 – February 2026  
Grade: 1.9  

---

## Author

Anurag Rathore  
anuragakrathore@gmail.com  
linkedin.com/in/anurag1017  
anurag101723.github.io
