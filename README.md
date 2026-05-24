# 🔬 Explainable AI for Strategic Decision-Making in SMEs

> **Master's Thesis** — M.Sc. Big Data & Business Analytics  
> FOM University of Applied Sciences, Essen, Germany · Grade: **1.9**

![Python](https://img.shields.io/badge/Python-3.12-blue?style=flat&logo=python&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-2.0-red?style=flat)
![SHAP](https://img.shields.io/badge/SHAP-0.44-orange?style=flat)
![LIME](https://img.shields.io/badge/LIME-0.2-yellow?style=flat)
![Status](https://img.shields.io/badge/Thesis-Grade%201.9-brightgreen?style=flat)

---

## 📌 Overview

Black-box machine learning models are powerful — but in high-stakes enterprise environments, **accuracy alone is not enough**. Decision-makers need to understand *why* a model recommends what it does before they can act on it with confidence.

This thesis designs, implements, and validates a full **Explainable AI (XAI) framework** for strategic decision support in enterprise contexts. By integrating **multi-source heterogeneous data** with state-of-the-art interpretability tools — SHAP and LIME — the framework bridges the gap between predictive performance and human-understandable reasoning.

The research addresses a critical question:

> *How can explainable AI be systematically integrated into enterprise decision pipelines to achieve both high predictive accuracy and full model transparency?*

---

## 🎯 Research Objectives

1. **Model Performance** — Develop high-accuracy predictive models using Random Forest and XGBoost across heterogeneous enterprise data
2. **Interpretability** — Apply SHAP and LIME to produce both global and local explanations for every prediction
3. **Stakeholder Usability** — Ensure non-technical decision-makers can act on model outputs with confidence
4. **Framework Validation** — Validate the XAI pipeline across multiple decision contexts and data types

---

## 🏆 Key Contributions

| Contribution | Description |
|---|---|
| XAI Pipeline | End-to-end framework from raw data to interpretable prediction |
| Dual Explainability | SHAP for global feature ranking + LIME for local case-level explanation |
| Multi-source Integration | Heterogeneous data fusion across structured and semi-structured sources |
| Stakeholder Layer | Plain-language explanation outputs designed for non-technical audiences |
| Comparative Analysis | Random Forest vs XGBoost performance and interpretability trade-offs |

---

## 🛠️ Tech Stack

| Category | Tools |
|---|---|
| Language | Python 3.12 |
| ML Models | XGBoost, Random Forest |
| Explainability | SHAP (TreeExplainer, SummaryPlot), LIME |
| Data Processing | Pandas, NumPy, Scikit-learn |
| Visualisation | Matplotlib, Seaborn |
| Environment | Jupyter Notebook |

---

## 🔍 Framework Architecture

```
┌─────────────────────────────────────────────────────┐
│                   DATA LAYER                        │
│   Multi-source heterogeneous enterprise data        │
│   (structured + semi-structured inputs)             │
└────────────────────┬────────────────────────────────┘
                     ↓
┌─────────────────────────────────────────────────────┐
│               PREPROCESSING LAYER                   │
│   Cleaning · Encoding · Scaling · Feature Selection │
└────────────────────┬────────────────────────────────┘
                     ↓
┌─────────────────────────────────────────────────────┐
│                  MODEL LAYER                        │
│   Random Forest  ←→  XGBoost                       │
│   Hyperparameter tuning · Cross-validation          │
└────────────────────┬────────────────────────────────┘
                     ↓
┌─────────────────────────────────────────────────────┐
│             EXPLAINABILITY LAYER                    │
│                                                     │
│   SHAP                        LIME                  │
│   ├── Global feature ranks    ├── Local explanations│
│   ├── Dependence plots        ├── Case-level why    │
│   └── Interaction effects     └── Feature weights  │
└────────────────────┬────────────────────────────────┘
                     ↓
┌─────────────────────────────────────────────────────┐
│              DECISION SUPPORT LAYER                 │
│   Human-readable outputs for non-technical          │
│   stakeholders · Audit trails · Compliance ready    │
└─────────────────────────────────────────────────────┘
```

---

## 🔑 Key Findings

- **XGBoost outperformed Random Forest** in predictive accuracy across all tested decision contexts
- **SHAP provided stable global explanations** — consistent feature rankings across data splits, critical for enterprise trust
- **LIME excelled at local explanations** — enabling case-by-case justification of individual predictions for stakeholders
- **Interpretability does not significantly reduce accuracy** — the XAI framework achieved competitive performance vs black-box baselines
- **Administrative and contextual variables** frequently ranked among top predictors, highlighting systemic factors beyond raw operational data
- The framework is **deployment-ready** — runtime efficiency supports near-real-time decision support integration

---

## 📐 Why XGBoost + SHAP + LIME?

| Method | Why Used |
|---|---|
| **XGBoost** | Superior performance on structured tabular data; handles missing values natively |
| **Random Forest** | Robust baseline; natural feature importance scores; lower overfitting risk |
| **SHAP** | Theoretically grounded (game theory); consistent global + local attribution |
| **LIME** | Model-agnostic; intuitive local approximations; accessible to non-technical users |

---

## 📁 Repository Structure

```
msc-thesis-xai-decision-making/
│
├── thesis_xai_framework.ipynb     # Main implementation notebook
├── README.md                      # Project documentation
```

---

## 🚀 How to Run

1. Clone the repository
```bash
git clone https://github.com/Anurag101723/msc-thesis-xai-decision-making.git
cd msc-thesis-xai-decision-making
```

2. Install dependencies
```bash
pip install pandas numpy scikit-learn xgboost shap lime matplotlib seaborn
```

3. Open the notebook
```bash
jupyter notebook thesis_xai_framework.ipynb
```

---

## 📚 Academic Context

**Program:** M.Sc. Big Data & Business Analytics  
**Institution:** FOM University of Applied Sciences, Essen, Germany  
**Period:** October 2025 – February 2026  
**Grade:** 1.9  

**Research Domain:** Explainable Artificial Intelligence (XAI) · Decision Support Systems · Enterprise Analytics

---

## 👤 Author

**Anurag Rathore**  
M.Sc. Big Data & Business Analytics — FOM University of Applied Sciences  
📧 anuragakrathore@gmail.com  
🔗 [LinkedIn](https://linkedin.com/in/anurag1017) · [Portfolio](https://Anurag101723.github.io)

---

*"The goal is not just to predict — it is to explain, justify, and earn trust."*
