# Telco Customer Churn — Analysis & Modeling

End-to-end analysis of the Telco Customer Churn dataset: data cleaning, EDA, churn prediction models, and customer segmentation.

## Repository structure

- `01_EDA_y_Limpieza.ipynb`  
  Data loading, cleaning, feature engineering, and exploratory analysis.

- `02_Modelos.ipynb`  
  Supervised modeling for churn prediction (train/test, evaluation metrics, model comparison).

- `03_Clustering.ipynb`  
  Unsupervised segmentation (clustering) to identify customer groups and insights.

- `Telco_customer_churn_DATASET.xlsx`  
  Dataset used in the notebooks (public source).

## How to run

1. Clone this repository.
2. Create a Python environment (Anaconda recommended).
3. Install dependencies (typical stack):
   - pandas, numpy
   - matplotlib, seaborn
   - scikit-learn
   - imbalanced-learn (if used)
4. Open Jupyter and run notebooks in order:
   - `01_EDA_y_Limpieza.ipynb`
   - `02_Modelos.ipynb`
   - `03_Clustering.ipynb`

> Note: Some intermediate artifacts (e.g., `.pkl` files) are not tracked to keep the repo clean and reproducible.  
> If a notebook expects a `.pkl`, re-run the previous notebook to generate it.

## Presentation / project context

- Project presentation (Notion): **https://www.notion.so/Osi-n-Jorge-Lezcano-2da5af0a537481b1b948e38da94fcfb9?source=copy_link#2da5af0a53748092a00be9c7f2e00da7**

## Notes

- Paths are relative so the project can be executed from the repository root.
- This project was developed and executed in Jupyter (Anaconda on Windows), but it should run on any standard Python environment.
