# Assignment-2
# 📊 Customer Churn Prediction using Logistic Regression

## 📌 Objective

The objective of this project is to develop a **Logistic Regression** model to predict whether a telecommunications customer is likely to **churn (leave the service)** based on demographic information, account details, and subscribed services. This project demonstrates the complete machine learning workflow including data preprocessing, feature encoding, model training, evaluation, and interpretation of results.

---

## 📂 Dataset Link

**Dataset Name:** Telco Customer Churn Dataset

**Source:** https://www.kaggle.com/datasets/blastchar/telco-customer-churn

The dataset contains customer demographic information, account details, subscribed services, and the target variable **Churn**.

---

## 🛠️ Libraries Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- KaggleHub

---

## ⚙️ Methodology

The following steps were performed during the implementation:

1. Imported the required Python libraries.
2. Loaded the dataset using **KaggleHub**.
3. Explored the dataset and identified numerical and categorical features.
4. Checked and handled missing values.
5. Converted categorical variables into numerical values using **Label Encoding**.
6. Removed unnecessary columns such as **customerID**.
7. Split the dataset into **80% training** and **20% testing** sets.
8. Built a **Logistic Regression** model.
9. Predicted customer churn on the test dataset.
10. Evaluated the model using:
    - Accuracy Score
    - Precision
    - Recall
    - F1-Score
    - Confusion Matrix

---

## 📊 Results

The Logistic Regression model was successfully trained and tested on the Telco Customer Churn dataset.

## 📊 Results

The Logistic Regression model was successfully trained and evaluated on the **Telco Customer Churn Dataset**.

### Evaluation Metrics

| Metric | Score |
|---------|------:|
| **Accuracy** | **82%** |
| **Precision** | **68%** |
| **Recall** | **58%** |
| **F1-Score** | **62%** |

### Classification Report

| Class | Precision | Recall | F1-Score | Support |
|------|----------:|-------:|---------:|--------:|
| **No Churn (0)** | 0.86 | 0.90 | 0.88 | 1036 |
| **Churn (1)** | 0.68 | 0.58 | 0.62 | 373 |

**Overall Accuracy:** **82%**

A **Confusion Matrix** was generated to visualize the model's classification performance.

### Observations

- The model achieved an overall **accuracy of 82%**, indicating good performance in predicting customer churn.
- It performed very well in identifying customers who **did not churn** (Class 0), with an F1-score of **0.88**.
- The model was less effective at identifying customers who **did churn** (Class 1), with a recall of **58%**, meaning some actual churn cases were missed.
- The weighted average F1-score of **0.81** suggests that the model performs well overall despite the imbalance between churn and non-churn customers.
---

## ✅ Conclusion

This project successfully implemented a Logistic Regression model for customer churn prediction. The preprocessing steps, including handling missing values and encoding categorical variables, enabled the model to learn meaningful patterns from the dataset. The evaluation metrics indicate that Logistic Regression provides reliable performance for predicting customer churn. Features such as contract type, monthly charges, tenure, and internet services significantly influence whether a customer is likely to leave. However, Logistic Regression assumes a linear relationship between features and the target variable, which may limit its ability to capture more complex customer behavior. More advanced machine learning algorithms such as Random Forest or XGBoost may achieve higher predictive performance.

---

## 📁 Project Structure

```
Assignment-2
│── Assignment-2.ipynb
│── README.md
```

---

## ▶️ How to Run

1. Clone this repository.
2. Open `Assignment-2.ipynb` in Google Colab or Jupyter Notebook.
3. Install the required dependencies if needed.

```bash
pip install kagglehub[pandas-datasets]
```

4. Run all notebook cells sequentially.
5. View the evaluation metrics and confusion matrix.

---
