# TBM_net-penetration-rate_tunnelling-himalayas_ML 
### TBM Penetration Rate Prediction in Himalayan Geology Using Machine Learning (ML) Techniques

**Authors:** Tek Bahadur Katuwal & Krishna Kanta Panthi  
**Institution:** Norwegian University of Science and Technology (NTNU)
**Published in:** *Rock Mechanics and Rock Engineering (2025)* 
**DOI:** [https://doi.org/10.1007/s00603-025-05044-z](https://doi.org/10.1007/s00603-025-05044-z)

---

## 📚 Table of Contents
1. [Overview](#1-overview)  
2. [Key Objectives](#2-key-objectives)  
3. [Database Availability](#3-database-availability)  
4. [Repository Structure](#4-repository-structure)  
5. [Data & Methodology](#5-data--methodology)  
6. [Key Findings](#6-key-findings)  
7. [Insights](#7-insights)  
8. [Conclusions](#8-conclusions)

---

## 1. Overview
This repository presents a **machine learning (ML)-based framework** for **TBM penetration rate prediction** in the challenging geological conditions of the Himalayas. The study utilizes **TBM operational data from the Bheri Babai Diversion Multipurpose (BBDM) Project in Nepal**.

### Key Highlights
- Machine learning (ML)-based model developed to predict **TBM net penetration rate (PRnet)**.  
- **TBM operational parameters** and **geological conditions** are utilized as input parameters.  
- Prediction model incorporates **data anomalies** associated with complex geological environments.  
- Impact of input features on TBM net penetration rate evaluated using the **SHAP method**.  
- **Risk of TBM jamming** assessed based on machine parameters and geological conditions.

---

## 2. Key Objectives
Develop a well-structured **Machine Learning (ML)-based framework** to predict **TBM net penetration rate (PRnet)** in complex geological environments.

---

## 3. Database Availability
Due to project confidentiality, the dataset **cannot be publicly shared**.

**Details:**
- **Source:** Bheri Babai Diversion Multipurpose (BBDM) Project, Nepal  
- **Size:** 8,614 TBM cycle datasets with corresponding mapped geological parameters  

---

## 4. Repository Structure
```
TBM_net-penetration-rate_tunnelling-himalayas_ML/
│
├── Data Analysis and Visualisation.ipynb
│     (Script that produces general dataset info, Pearson Correlation Analysis,
│      feature importance, Box–Whisker & Violin Plot, histogram distributions)
│
├── Engineering Geological Assessment.ipynb
│     (Visualizations of lithology, rock mass class, weathering grade,
│      and rock strength distributions)
│
├── Hyperparameter optimization/
│     (Scripts for tuning optimal hyperparameters for selected regression models)
│
├── ML model/
│     ├── Regression model training and testing scripts
│     └── Model performance evaluation
│
├── SHAP_Model Interpretability Analysis.ipynb
│     (Model interpretability and feature influence analysis using SHAP)
│
├── Discussion of TBM Net Penetration Rate Performance Results.ipynb
│     (Analysis of TBM performance in different lithology, rock mass quality,
│      weathering, rock strength, and TBM jamming or thrust sections)
│
└── README.md
```
---

## 5. Data & Methodology

- **Dataset:** 8,614 real-time TBM cycle data points from a 12 km tunnel  
- **Input Features:**  
  - Geological: Rock mass rating (RMR), lithology, weathering, rock strength  
  - Machine: Torque, thrust, cutterhead speed (CRS), penetration rate (PRchd)
- **ML Models Used:**  
  - *Non-Ensemble:* SVR, KNN, Decision Tree  
  - *Ensemble:* Bagging, Random Forest, XGBoost, Stacking  
  - *Neural Network:* Artificial Neural Network (ANN)
- **Evaluation Metrics:** R², MAE, RMSE, MAPE  
- **Interpretability Tool:** SHAP (Shapley Additive Explanations)

---

## 6. Key Findings

- **Best Models:** ANN and Stacking ensemble achieved the highest **R² of 0.94**.  
- **SHAP Analysis:**  
  - Most influential features: Cutterhead penetration rate (PRchd), cutterhead speed (CRS), rock mass rating (RMR), torque, thrust.  
  - Geological features (lithology, rock strength) also contributed but with lesser influence.  
- **Outliers:** Retained instead of removed to capture critical events such as **TBM jamming**.  
- **Critical Sections:** Torque and thrust fluctuations are strong indicators of **potential jamming zones**.

---

## 7. Insights

- **Geological Complexity:** Himalayan geology exhibits extreme variability due to tectonic activity, making TBM performance prediction challenging.  
- **ML Advantage:** Machine learning models outperform traditional empirical/statistical approaches in capturing nonlinear dependencies and handling complex datasets.  
- **Safety & Efficiency:** The framework aids in **early risk detection**, **optimization of TBM operations**, and **enhancement of tunneling safety**.

---

## 8. Conclusions

- ML-based models can accurately predict TBM performance in **complex geological environments**.  
- Integration of **geological and machine parameters** enhances model reliability.  
- The developed framework is **generalizable** but requires further validation using **data from other tunneling projects**.

---

**© 2025 Norwegian University of Science and Technology (NTNU)**  
*Authors: Tek Bahadur Katuwal & Krishna Kanta Panthi*
