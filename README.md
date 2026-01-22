# Personalized Early Prediction of Weight Loss Success using Transfer Learning and Explainable GRU-Attention

This repository contains the implementation for the research paper:

**"Personalized Early Prediction of Weight Loss Success Using Transfer Learning and Explainable GRU-Attention Networks"**

---

## 🚀 Objective

To build an early clinical prediction model that identifies whether a patient will successfully lose weight using:

✓ Transfer Learning (cross-cohort)  
✓ Attention-based Deep Learning  
✓ Explainable AI (SHAP + Attention Maps)

---

## 🧠 Methodology Overview

The pipeline consists of:

1. **Pretraining**
   - Dataset: **CALERIE clinical weight-loss dataset**
   - Architecture: **Bidirectional GRU + Self-Attention**

2. **Fine-tuning**
   - Dataset: **Independent Iranian cohort**
   - Domain Adaptation for population shift

3. **Explainability**
   - SHAP values for feature contribution
   - Attention maps for temporal interpretation

---

## 📈 Key Results

| Model                                | AUC     | Notes                               |
|-------------------------------------|---------|-------------------------------------|
| GRU-Attention (local baseline)      | 0.953   | No transfer learning                |
| TL-GRU-Attention (proposed)         | 0.991   | ↓ variability (6× improvement)      |
| Early Prediction (W1–W2 features)   | 0.969   | Supports proactive intervention     |

---
## 📈 Early Prediction Performance (Iran Cohort)
![Early AUROC Trends](figures/early_auroc_trend.png)

## 🔍 Attention Heatmap (Explainability)
![Attention Heatmap IRAN](figures/attention_heatmap_iran.png)



## 📂 Repository Structure

