# SyriaTel Customer Churn Prediction

## Business Problem

SyriaTel, a telecommunications provider, wants to identify customers who are likely to stop using their services ("churn") in the near future. Retaining customers is more cost-effective than acquiring new ones, so predicting churn early allows for targeted interventions like loyalty offers or personalized support.

---

## Project Objective

This project aims to build a binary classification model to predict whether a customer will churn or not, using historical customer behavior and usage data. The final model should provide actionable insights to help SyriaTel reduce churn rates and improve customer retention strategies.

---

## Methodology

* **Business Understanding**: Identified churn prediction as the key objective tied to business revenue loss.
* **Data Preprocessing**: Cleaned, encoded, and prepared the dataset for modeling.
* **Exploratory Data Analysis (EDA)**: Uncovered patterns and relationships in the data that correlate with churn.
* **Modeling**: Built and compared Logistic Regression and Random Forest models.
* **Evaluation**: Assessed model performance using accuracy, precision, recall, F1-score, and ROC-AUC.
* **Interpretation**: Analyzed feature importance to highlight key churn drivers.

---

## Dataset

The dataset contains 21 features and one target (`Churn`). Key features include:

* Customer account length, subscription type, usage patterns, complaints, and service calls.
* Target variable: `Churn` (Yes = customer left, No = customer stayed)

---

## Models Used

* **Baseline**: Logistic Regression
* **Improved**: Random Forest Classifier

  > Random Forest was selected for its robustness, accuracy, and interpretability via feature importance.

---

## Results

* **Random Forest Accuracy**: \~92%
* **Top Predictive Features**: Contract Type, Tenure, Number of Complaints, Data Usage, and Monthly Charges
* **ROC-AUC Score**: 0.93

---

## Key Insights

* Customers on month-to-month contracts and those with high complaint counts are more likely to churn.
* Longer-tenure customers are more loyal and should be prioritized with retention programs.
* Usage patterns and service-related issues are key churn indicators.

---

## Recommendations

* Offer loyalty benefits to at-risk customers with high tenure.
* Proactively contact customers with frequent complaints or high service call volumes.
* Design flexible plans for customers on month-to-month contracts to increase satisfaction.

---

## How to Run

```bash
# Install dependencies
pip install pandas scikit-learn matplotlib seaborn

# Run the notebook
jupyter notebook SyriaTel_Customer_Churn_Project.ipynb
```

---