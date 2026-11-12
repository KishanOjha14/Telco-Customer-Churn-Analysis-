# Telco Customer Churn Analysis

By **Kishan Kumar Ojha**

![Python](https://img.shields.io/badge/Python-3.x-blue.svg)
![SQL Server](https://img.shields.io/badge/SQL%20Server-Data%20Cleaning-blue.svg)
![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-yellow.svg)
![scikit-learn](https://img.shields.io/badge/scikit--learn-Random%20Forest-orange.svg)

---

## 📋 Project Overview

This project explores and analyzes the **Telco Customer Churn dataset** from Kaggle to understand churn behavior and build a machine learning model to predict customer retention. The workflow includes data cleaning, interactive dashboarding, and classification modeling using the **Random Forest** algorithm.

### 🔑 Objectives
- Clean and preprocess the Telco customer dataset using SQL Server.
- Visualize churn patterns via an interactive Power BI dashboard.
- Train a Random Forest classifier to predict customer churn.
- Evaluate model performance and surface actionable business insights.

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|------|---------|
| **SQL Server** | Data cleaning and preprocessing |
| **Power BI** | Interactive dashboards and visualizations |
| **Python (Jupyter Notebook)** | Machine learning (Random Forest), feature analysis, evaluation |
| **Libraries** | pandas, matplotlib, seaborn, scikit-learn |

---

## 📊 Dataset

The dataset is sourced from Kaggle:  
🔗 [Telco Customer Churn – Kaggle](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)

It contains detailed information about customers, their services, account details, and churn status.

### Data Cleaning (SQL)
- Handled missing values
- Converted the `TotalCharges` column from string to float
- Mapped the `Churn` column to binary values (`Yes = 1`, `No = 0`)

The cleaned dataset was imported into Power BI for dashboarding, then into Jupyter Notebook for modeling.

---

## ⚙️ Model Configuration

- **Algorithm:** Random Forest Classifier
- **Train-Test Split:** 80:20
- **Estimators:** 100
- **Random State:** 42

### Model Evaluation

| Metric | Class 0 (Retained) | Class 1 (Churned) |
|--------|--------------------|-------------------|
| Precision | 83% | 67% |
| Recall | 92% | 46% |
| F1-Score | 87% | 55% |

**Overall Accuracy: 80%**

---

## 🔍 Key Insights from Research Questions

1. **Tenure:** Churned customers stay for an average of **18 months**, while retained customers stay around **38 months** — longer-tenured customers are less likely to churn.
2. **Internet Service:** Fiber optic users show the highest churn rate (~42%), DSL users churn moderately (~20%), and customers without internet service churn the least (~6%).
3. **Contract Type:** Month-to-month contract users churn the most (~45%), whereas one-year (~12%) and two-year (~2%) contract users are more loyal — long-term contracts reduce churn.
4. **Lifetime Value (LTV):** Retained customers have significantly higher LTV than churned ones — churned users generate less revenue over time.
5. **Feature Influence:** Internet Service and Contract Type had the strongest influence on LTV, while Gender had negligible impact.

---

## 💼 Business Insights & Recommendations

| # | Insight | Recommendation |
|---|---------|----------------|
| 1 | Month-to-month plans have the highest churn (~45%); two-year contracts have the lowest (~2%). | Offer loyalty rewards, discounts, or perks to encourage longer contract commitments. |
| 2 | Fiber optic users show the highest churn (~42%) among all internet service types. | Investigate pricing or service quality concerns; offer customized plans or support. |
| 3 | Churned customers typically leave within the first 18 months. | Focus on onboarding, regular engagement, and first-year incentives. |
| 4 | Contract type and Internet Service significantly affect LTV; gender has little impact. | Use segmentation and upselling strategies to improve LTV among low-value customers. |
| 5 | Better service support is linked to higher tenure and retention. | Introduce tech support plans and flag high-risk accounts for proactive outreach. |
| 6 | The Random Forest model predicts churn with 80% accuracy. | Use the model to trigger retention campaigns before customers decide to leave. |

---

## 📁 Repository Structure

```
Customer-Churn-Analysis-main/
├── README.md
├── Telco-Customer-Churn.csv          # Raw dataset from Kaggle
├── Customer-Churn_Telco_Clean.csv    # Cleaned dataset (SQL)
├── Customer_Churn-prediction-analysis.ipynb      # ML analysis notebook
├── Customer_Churn-prediction-analysis-executed.ipynb  # Executed notebook
└── Customer_Churn-prediction-analysis-executed.html   # Exported HTML report
```

---

## 🚀 Getting Started

### Prerequisites
- Python 3.x
- Jupyter Notebook / JupyterLab
- SQL Server
- Power BI Desktop

### Python Libraries
```bash
pip install pandas matplotlib seaborn scikit-learn
```

### Usage
1. Clone the repository:
   ```bash
   git clone https://github.com/KishanOjha14/Telco-Customer-Churn-Analysis-.git
   cd Telco-Customer-Churn-Analysis-
   ```
2. Open `Customer_Churn-prediction-analysis.ipynb` in Jupyter Notebook to reproduce the machine learning analysis.
3. Load `Customer-Churn_Telco_Clean.csv` into Power BI to explore the interactive dashboard.
4. Review `README.md` for key findings and business recommendations.

---

## 📄 License

This project is for educational and analytical purposes.

---

## 🙋‍♂️ Author

**Kishan Kumar Ojha**  
Email: kishanojha47@gmail.com  
GitHub: [KishanOjha14](https://github.com/KishanOjha14)