### HR Analytics: Predicting and Understanding Employee Attrition

## Project Overview

This project focuses on analyzing and predicting employee attrition using a dataset of employee information. By applying Exploratory Data Analysis (EDA) and machine learning models, the goal is to identify the key factors that lead to employees leaving the company and to build a predictive tool that can identify employees at high risk of attrition. The final output includes a risk-based segmentation of employees, which can empower HR to take proactive measures to retain talent.

## Key Questions Addressed

* What is the overall attrition rate of the company's workforce?
* Which departments and salary levels are most affected by attrition?
* How do factors like satisfaction level, project count, and tenure influence an employee's decision to leave?
* Can a machine learning model accurately predict which employees are likely to leave?

## Data Source

The analysis is based on the `employe.csv` file, which contains various attributes about employees, including their professional details and whether they have left the company (`left`).

---

## Analysis and Findings

### 1. Exploratory Data Analysis (EDA)

* **Overall Attrition:** The total attrition rate is **14.9%**, with 2,381 out of 15,999 employees having left.
* **Department Attrition:** The **sales**, **technical**, and **support** departments have the highest number of employees who have left.
* **Salary and Attrition:** Employees with **low** and **medium** salaries show a significantly higher attrition rate than those with high salaries.
* **Project Count Impact:** Employees working on **2, 6, or 7 projects** have the highest attrition rates, and the attrition rate for employees with less than three projects is a notable **40.06%**.
* **Key Indicators:** Employees who left typically had a lower satisfaction level, higher average monthly hours, and a tenure of 3-6 years, with a peak at 5 years. The analysis also highlighted a group of high-performing, overworked employees with high evaluation scores but low satisfaction who were prone to leaving.

---

### 2. Predictive Modeling

* **Models Used:** Several machine learning models were trained to predict employee attrition, including:
    * **Logistic Regression**
    * **Support Vector Machine (SVM)**
    * **K-Nearest Neighbors (KNN)**
    * **Decision Tree**
    * **AdaBoost**
    * **Gradient Boosting**
    * **XGBoost**
    * **Multi-layer Perceptron (MLP)**
* **Performance:** The **XGBoost** model demonstrated the best performance, achieving an accuracy of **99.2%** and a ROC-AUC score of **0.994** on the hold-out test set.

---

### 3. Employee Churn Risk Segmentation

The final model was used to predict the churn probability for every employee, segmenting them into three risk buckets:

| Risk Bucket | Attrition Rate | Description |
| :--- | :--- | :--- |
| **Low** | **1.3%** | Employees with a very low probability of leaving. |
| **Medium** | **11.4%** | Employees with a moderate risk of attrition. |
| **High** | **97.4%** | Employees with a very high likelihood of leaving. |

This segmentation provides actionable insights for HR to focus retention efforts on the most at-risk individuals.

## Conclusion

This project successfully demonstrates how data analytics and machine learning can be leveraged to gain deep insights into employee attrition. The predictive model provides a powerful tool for proactively identifying and addressing the root causes of churn, enabling the organization to improve employee retention and overall workforce stability.
