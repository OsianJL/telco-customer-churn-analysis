# Telco Customer Churn Project — Prediction & Segmentation

End-to-end data science project focused on customer churn analysis in the telecommunications domain.  
The project combines **supervised churn prediction** with **unsupervised customer segmentation** to support actionable, business-oriented retention strategies.

---

## Project Overview

The objective of this project is twofold:

- **Predict customer churn** using a supervised machine learning model, prioritizing churn detection while maintaining operational usefulness.
- **Segment customers into meaningful groups** using unsupervised learning, enabling targeted and differentiated business actions.

The project emphasizes:
- methodological rigor (proper train/test split, SMOTE applied only on training data),
- model interpretability,
- and business relevance over metric optimization alone.

---

## Main Results

- The final churn model identifies **approximately 78% of customers who will churn**, while maintaining a balanced level of false alarms, making it suitable for targeted retention actions.
- Customer segmentation reveals **four distinct and interpretable customer profiles** with clearly differentiated churn risk and behavioral patterns.

---

## Repository Structure

- `Telco_Customer_Churn_Project.ipynb`  
  Single, consolidated notebook including:
  - Data cleaning and exploratory data analysis (EDA)
  - Feature selection and preparation
  - Supervised churn modeling (Logistic Regression, Tree-based models, threshold analysis)
  - Model evaluation and selection
  - Unsupervised customer segmentation (KMeans)
  - Cluster interpretation and business recommendations

- `Telco_customer_churn_DATASET.xlsx`  
  Dataset used in the analysis (publicly available source).

---

## Methodology Summary

### Churn Prediction
- Binary target: `Churn Value`
- Train/test split with class imbalance handling using **SMOTE applied only to the training set**
- Multiple models evaluated (Logistic Regression, Decision Tree, Random Forest, XGBoost)
- Final model selection based on recall, F1 score, interpretability, and business usability
- Decision threshold explicitly analyzed and justified

### Customer Segmentation
- Independent feature selection focused on behavior, value, services, and demographics
- Full feature scaling prior to clustering
- KMeans clustering with:
  - Elbow method
  - Silhouette score
- Final choice of **K = 4 clusters**
- Cluster interpretation performed using original (non-scaled) variables and churn rates for validation

---

## How to Run the Project

1. Clone this repository.
2. Create a Python environment (Anaconda recommended).
3. Install dependencies:
   - pandas
   - numpy
   - matplotlib
   - seaborn
   - scikit-learn
   - imbalanced-learn
4. Open Jupyter Notebook and run:
   - `Telco_Customer_Churn_Project.ipynb`

All steps are executed sequentially within the same notebook.

---

## Potential Extensions

- Operationalization of the churn model via an API (e.g., FastAPI)
- Integration with Power BI to enable interactive exploration of churn risk and customer segments
- Cost-sensitive optimization of decision thresholds
- Validation using alternative clustering techniques

---

## Notes

- The project was developed using Jupyter Notebook (Anaconda, Windows), but it should run on any standard Python environment.
- Paths are relative to ensure reproducibility.
- The focus of the project is analytical rigor and business interpretability rather than leaderboard optimization.
