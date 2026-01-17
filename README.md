# InsightX-Data-Driven-Employee-Performance-Attrition-Analytics

# InsightX: Data-Driven Employee Performance & Attrition Analytics

![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)
![Scikit-Learn](https://img.shields.io/badge/Machine_Learning-Scikit--Learn-orange.svg)
![NLP](https://img.shields.io/badge/NLP-VADER%20%7C%20BERT-green.svg)
![Status](https://img.shields.io/badge/Project_Status-Completed-brightgreen.svg)

## 📌 Project Overview
**InsightX** is an end-to-end HR Analytics solution designed to predict employee turnover and identify burnout drivers using a hybrid approach of statistical modeling and Natural Language Processing (NLP).

By analyzing both structured data (tenure, pay, performance) and unstructured data (feedback text), InsightX provides leadership with a clear picture of why employees leave and the financial return on implementing retention strategies.

---

## 🛠️ Tech Stack
* **Environment:** Google Colab
* **Language:** Python (Pandas, NumPy)
* **Machine Learning:** Scikit-Learn (Random Forest, Logistic Regression)
* **NLP:** NLTK, VADER, Transformers (BERT)
* **Visualization:** Matplotlib, Seaborn, Power BI
* **Data Generation:** Faker Library

---

## 🚀 Key Features & Workflow

### 1. Synthetic Data Engineering
Created a robust HR dataset using the `Faker` library, simulating realistic organizational structures including:
* **Demographics:** Job Roles, Departments, Monthly Pay, and Tenure.
* **Performance:** Satisfaction Scores and Performance Ratings.
* **Unstructured Data:** Synthetic employee feedback paragraphs for sentiment mining.

### 2. Predictive Attrition Modeling
Developed a classification pipeline to identify high-risk employees.
* **Performance:** Achieved **73% Accuracy** with balanced precision and recall.
* **Driver Analysis:** Identified `SatisfactionScore`, `MonthlyPay`, and `TenureMonths` as the primary predictors of employee exit.



### 3. Psycholinguistic Burnout Mapping (NLP)
Integrated a specialized text analytics workflow to detect "hidden" attrition drivers:
* **VADER Sentiment:** Categorized general feedback as Positive, Neutral, or Negative.
* **Burnout Detection:** Mapped specific keywords (e.g., "drained," "overwhelmed," "stagnant") to exhaustion and cynicism categories to flag employees nearing burnout before their performance drops.

### 4. Retention ROI Calculator
A dedicated financial logic module that translates model predictions into business value.
* **Metric:** Calculated the net savings of retention programs by comparing turnover costs (recruitment, onboarding) vs. the cost of intervention.
* **Impact:** Demonstrated how identifying at-risk talent can lead to a positive ROI within a single fiscal year.

---

## 📊 Dashboard & Visualization
The project data is optimized for Power BI integration, focusing on:
* **Departmental Risk Heatmaps:** Identifying which teams are under the most pressure.
* **Sentiment vs. Tenure:** Visualizing how employee morale shifts over time.
* **Attrition Probability:** A ranked list of at-risk employees for HR intervention.



---

## 📂 Project Structure
```bash
├── InsightX_Colab_Notebook.ipynb  # Full Python implementation
├── hr_analytics_dataset.csv       # Raw synthetic dataset
├── dashboard_data_export.csv      # Processed data for Power BI
└── README.md                      # Project documentation
