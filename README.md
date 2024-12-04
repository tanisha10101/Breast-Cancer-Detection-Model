# Breast Cancer Detection using Machine Learning  

Breast cancer is the most common cancer among women worldwide, accounting for a significant portion of all cancer cases. This project utilizes machine learning techniques to classify tumors as **malignant** (cancerous) or **benign** (non-cancerous), leveraging the Breast Cancer Wisconsin (Diagnostic) Dataset. Through this project, we aim to simplify and enhance the process of cancer diagnosis by developing highly accurate predictive models.  

---

## Table of Contents  
1. [Introduction](#introduction)  
2. [Dataset Overview](#dataset-overview)  
3. [Objective](#objective)  
4. [Features of the Dataset](#features-of-the-dataset)  
5. [Machine Learning Approach](#machine-learning-approach)  
6. [Results](#results)  
7. [Conclusion](#conclusion)  
8. [How to Use This Project](#how-to-use-this-project)  

---

## Introduction  

Breast cancer occurs when abnormal changes in cell growth lead to the formation of a malignant tumor in the breast. As the tumor matures, it can metastasize (spread) to other parts of the body through the lymphatic system, creating new tumors and exacerbating the disease. While breast cancer is more common in women, it can also occur in men, albeit rarely.  

Early and accurate detection of breast cancer is critical for effective treatment and better outcomes. This project employs machine learning techniques, particularly **Support Vector Machines (SVM)**, to achieve high accuracy in classifying tumors based on diagnostic features derived from mammograms.  

---

## Dataset Overview  

### Source  
The dataset used is the **Breast Cancer Wisconsin (Diagnostic) Dataset**, available through the Scikit-learn library.  

### Key Statistics  
- **63%** of the diagnoses are benign.  
- The dataset contains a wide range of features such as radius, texture, perimeter, area, and smoothness.  

### Prevalence by Region (2018):  
- **Asia**: 59% of the global population, 39% of new cases, 44% of deaths.  
- **Africa**: 15% of the global population, 8% of new cases, 12% of deaths.  
- **US and Canada**: 5% of the global population, 15% of new cases, 9% of deaths.  

### Incidence Rates per 100,000 Women:  
- **Highest Incidence**: Netherlands (95.3), France (94.6), US (90.6).  
- **Lowest Incidence**: Thailand (25.6), Algeria (29.8), India (30.9).  

---

## Objective  

The primary objective of this project is to develop machine learning models that:  
1. Classify breast cancer tumors as **malignant** or **benign**.  
2. Fine-tune hyperparameters to optimize accuracy.  
3. Compare the performance of various classification algorithms.  

---

## Features of the Dataset  

The dataset contains diagnostic features derived from digitized images of a breast mass.  

### Key Columns:  
1. **Diagnosis**: Malignant (M) or Benign (B).  
2. **Mean Features**: Radius, Texture, Perimeter, Area, Smoothness, Compactness, Concavity, Symmetry, etc.  
3. **Standard Error (SE) Features**: Variability in the measurements.  
4. **Worst Features**: The largest value recorded for each measurement.  

---

## Machine Learning Approach  

### Techniques Used:  
1. **Data Preprocessing**:  
   - Normalization to ensure all features are on the same scale.  
   - Handling missing values or outliers (if applicable).  

2. **Model Development**:  
   - Algorithms tested include **SVM**, **Logistic Regression**, and **Random Forest**.  
   - Hyperparameter optimization for SVM using parameters `C` and `Gamma`.  

3. **Evaluation Metrics**:  
   - Accuracy  
   - Precision  
   - Recall  

4. **Feature Importance**:  
   - The most critical features were:  
     - **Texture Mean**  
     - **Concavity Mean**  
     - **Fractal Dimension (SE)**  
     - **Worst Concavity**  
     - **Mean of Symmetry**  

---

## Results  

- The **Support Vector Machine (SVM)** model achieved the highest accuracy of **97%** after hyperparameter tuning.  
- Precision scores reached **100%**, indicating highly reliable predictions for malignant tumors.  
- Key insights derived from the dataset:  
  - Malignant tumors tend to have higher mean values for **radius**, **perimeter**, and **compactness**.  
  - No statistically significant difference in features like **fractal dimension** and **texture SE** between malignant and benign tumors.  

---

## How to Use This Project  

1. **Clone the Repository**:  
   ```bash  
   git clone <repository-link>  
   cd <repository-folder>  
---

## Conclusion  

This project demonstrates the power of machine learning in medical diagnosis, particularly for breast cancer detection. By leveraging SVM, we were able to achieve a near-perfect accuracy score. This technology has the potential to reduce diagnostic errors and assist healthcare professionals in making informed decisions.  

---
