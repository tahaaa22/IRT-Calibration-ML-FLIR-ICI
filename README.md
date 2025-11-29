# IRT-Calibration-ML-FLIR-ICI
This repository contains the full machine-learning pipeline for calibrating two infrared thermograph devices (FLIR and ICI) against clinical oral thermometer measurements. The project was developed as part of the Medical Standards and Accreditation (SBES270) course at Cairo University.
Below is a **professional GitHub README** and a **repository name** suitable for your project.

## 📌 Project Overview

Infrared thermographs (IRTs) are widely used for non-contact elevated body temperature screening. However, their diagnostic accuracy depends heavily on proper calibration.

This project evaluates two thermal imaging devices:

- **IRT-1:** FLIR Camera  
- **IRT-2:** ICI Camera  

Using machine learning regression models, we calibrate each device to predict true oral temperature and compare their clinical performance.

---

## 🎯 Objectives

- Build calibration models that estimate oral temperature using facial temperature features.  
- Evaluate each device using machine learning regression techniques.  
- Compare FLIR vs. ICI through statistical and visual performance metrics.  
- Identify the most predictive facial regions (e.g., canthus, orbital).  
- Produce a final accuracy ranking.

---

## 📂 Repository Structure

```

IRT-Calibration-ML-FLIR-ICI/
│
├── data/                   
├── notebook/
│   └── Medical_device_calibration_software_Team_2.ipynb
└── README.md

````

## 🔬 Methodology Summary

### **1. Data Processing**
- Integrated multi-round measurements for each subject.  
- Cleaned missing and inconsistent values.  
- Normalized temperature features when necessary.

### **2. Feature Engineering**
- Extracted key facial regions: canthus, orbital, forehead, full-face max.  
- Created composite variables such as “mean canthus temperature”.

### **3. Machine Learning Models**
Each device was calibrated using:

- **Random Forest Regression**  
- **Gradient Boosting Regression**  
- **Support Vector Regression (SVR)**  

### **4. Evaluation Metrics**
- **MAE** – Mean Absolute Error  
- **RMSE** – Root Mean Squared Error  
- **MAPE** – Mean Absolute Percentage Error  
- **R²** – Coefficient of Determination  

---

## 📊 Visualizations

The notebook generates:

- Calibration scatter plots  
- Bland–Altman plots  
- Feature importance graphs  
- Residual plots  
- Performance comparison bar charts  

These visuals help assess accuracy and identify potential calibration bias.

---

## 🏆 Key Findings

- **FLIR outperformed ICI** across all core evaluation metrics.  
- **Canthus temperature** is the strongest predictor for core temperature.  
- Gradient Boosting Regression provided the best calibration performance.  
- Machine learning significantly improves IRT clinical accuracy.

---

## 🛠️ Tools & Technologies

- **Python**
- **Jupyter Notebook**
- **Pandas / NumPy**
- **Scikit-Learn**
- **Matplotlib / Seaborn**
- **SciPy**

---


Just tell me!
```
