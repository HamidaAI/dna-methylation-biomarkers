
# 🧬 DNA Methylation Analysis for Methylation Status Prediction

## Overview

DNA methylation is an epigenetic mechanism that regulates gene expression without altering the DNA sequence. Abnormal methylation patterns have been linked to many diseases, making them an important area of study in bioinformatics and precision medicine.

In this project, I explored a DNA methylation dataset containing genomic features related to CpG sites and trained machine learning models to predict methylation status. Beyond building predictive models, the project focused on understanding the data, interpreting model behavior, and comparing different algorithms from both a machine learning and biomedical perspective.

---

## Research Question

**Can genomic features describing CpG sites accurately predict DNA methylation status using machine learning?**

---

## Dataset

* **Dataset:** DNA Methylation Data – Epigenetic Biomarkers
* **Source:** https://www.kaggle.com/datasets/juanschafle/dna-methylation-data-epigenetic-biomarkers
* **Samples:** 1,000
* **Features:** 4 predictor variables and 1 target variable
* **Target Variable:** `methylation_status`

  * 0 = Unmethylated
  * 1 = Methylated

### Predictor Variables

* CpG Density
* Genomic Location
* Regulatory Score
* Conservation Score

The dataset is based on genomic characteristics associated with DNA methylation and was created for educational and machine learning applications in bioinformatics.

---

## Project Workflow

* Performed Exploratory Data Analysis (EDA)
* Verified data quality (missing values and duplicates)
* Explored feature distributions
* Investigated relationships between features
* Analyzed feature correlations
* Examined correlations between features and the target variable
* Trained multiple machine learning models
* Compared model performance
* Interpreted results from a biomedical perspective

---

## Models Trained

* Logistic Regression
* Decision Tree
* Random Forest

For the Decision Tree model, different tree depths were tested to study the effect of model complexity and overfitting.

---

## Model Comparison

| Model               | Test Accuracy | Interpretation                                                                       |
| ------------------- | ------------: | ------------------------------------------------------------------------------------ |
| Logistic Regression |       **97%** | Best overall performance; the dataset follows a relatively simple decision boundary. |
| Random Forest       |       **95%** | Strong performance with only a small degree of overfitting.                          |
| Decision Tree       |       **87%** | Overfitted the training data despite tuning tree depth.                              |

---

## Model Evaluation

The models were evaluated using:

* Accuracy
* Confusion Matrix
* Feature Importance
* Predicted Probability Distribution (Model Confidence)

The analysis also included comparing training and testing accuracy to assess overfitting.

---

## Key Findings

* Logistic Regression achieved the best overall performance on this dataset.
* Although feature-to-target correlations were only moderate, combining multiple genomic features allowed the models to achieve high predictive performance.
* Decision Trees were highly sensitive to model complexity and easily overfitted the training data.
* Random Forest reduced overfitting compared to a single Decision Tree while maintaining strong predictive performance.

---

## What I Learned

Through this project, I learned:

* How to perform Exploratory Data Analysis on biomedical datasets.
* How to evaluate data quality before model training.
* Why accuracy alone is not sufficient for evaluating machine learning models.
* Why false negatives are especially important in healthcare-related applications.
* How model complexity influences generalization and overfitting.
* Why simpler models can sometimes outperform more complex algorithms.
* How feature correlations can be interpreted when analyzing biomedical datasets.
* How to compare machine learning models beyond a single performance metric.

---

## Tools & Libraries

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* Jupyter Notebook

---

## About This Project

This project is part of my journey to build AI and data literacy in healthcare through hands-on analysis of biomedical datasets and machine learning.
