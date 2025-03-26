# fairml-xai-pipeline
This repository contains the code, analysis, and report for a research project focused on fairness and interpretability in machine learning.
# FairML-XAI: Fairness and Interpretability in Machine Learning

This repository accompanies a research project focused on improving fairness and transparency in machine learning models applied to socially sensitive domains. Using real-world datasets—the **UCI Adult Income** dataset and the **COMPAS** dataset—this project investigates **bias mitigation** through **class reweighting** and explains model behavior using **Explainable AI (XAI)** techniques like **SHAP**, **LIME**, and **Phi-2** natural language generation.

## Objectives
- Detect and quantify algorithmic bias in high-stakes datasets.
- Apply and evaluate **class reweighting** as a fairness intervention.
- Use **SHAP** and **LIME** to explain model predictions.
- Leverage **Phi-2**, a small language model, to translate complex model outputs into human-readable narratives.


## 🔍 Datasets

### 🧾 UCI Adult Income Dataset
- Binary classification task: Predict if income >$50K/year.
- Sensitive features: **gender**, **race**
- Imbalance noted: Only ~11% of women are labeled high-income vs. ~30% of men.

### ⚖️ COMPAS Dataset
- Risk assessment dataset for recidivism prediction.
- Sensitive feature: **race**
- Black defendants were **45% more likely** to be misclassified as high-risk compared to white defendants.

## ✅ Fairness Techniques

- **Class Reweighting**  
  Balances the influence of underrepresented groups during model training.

- **Fairness Metrics Evaluated**  
  - Equal Opportunity (primary)
  - Disparate Impact
  - Demographic Parity
  - Error Rate Parity

## 🔍 Explainable AI (XAI)

- **SHAP** (SHapley Additive Explanations)  
  Global and local feature attribution.

- **LIME** (Local Interpretable Model-Agnostic Explanations)  
  Local surrogate models to understand prediction rationale.

- **Phi-2**  
  Converts SHAP values into **natural language** for stakeholder-friendly explanations.

## 📈 Results Summary

| Dataset      | Metric        | Baseline | Reweighted |
|--------------|---------------|----------|-------------|
| Adult Income | TPR           | 0.447    | 0.830       |
| Adult Income | FNR           | 0.553    | 0.170       |
| COMPAS       | TPR           | 0.221    | 0.597       |
| COMPAS       | FNR           | 0.779    | 0.403       |

## 📘 Citation

If you use this work, please cite:

```bibtex
@misc{fairmlxai2025,
  title={FairML-XAI: Improving Fairness and Interpretability in Machine Learning},
  author={Wabella, Akinahom},
  year={2025},
  url={https://github.com/yourusername/fairml-xai}
}


