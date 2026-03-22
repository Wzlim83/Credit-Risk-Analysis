# 💼 Credit Risk Portfolio Analysis

This project demonstrates an **end-to-end credit portfolio analysis workflow** using synthetic SME loan data.
The objective is to **identify high-risk borrowers, assess portfolio exposure, and visualize risk clusters** using Python and Power BI.

---

## 🛠 Tools & Technologies

* **Python** – Pandas, NumPy, Matplotlib for data generation, cleaning, and analysis
* **Power BI** – Interactive dashboards and DAX measures
* **Excel / CSV** – Initial dataset exploration

---

## 📂 Project Workflow

### 1. Data Generation

A synthetic dataset was created to simulate a **loan portfolio dataset** for analytical purposes.

Fields included:

* `Borrower_ID`
* `Industry`
* `Loan_Amount`
* `Revenue`
* `Credit_Score`

Random data generation allows the project to replicate a **realistic portfolio analysis scenario**.

---

### 2. Data Cleaning & Preparation

The dataset was cleaned using Python to ensure data quality:

* Checked for **missing values**
* Replaced missing numeric values using **median imputation**
* Removed **duplicate borrower records**
* Standardized **text fields** (e.g., industry names)

---

### 3. Debt-to-Income (DTI) Calculation

A financial leverage indicator was created:

```
DTI = Loan_Amount / Revenue
```

Higher DTI indicates **higher financial leverage and potential repayment risk**.

---

### 4. Risk Category Classification

Borrowers were segmented into risk groups based on **credit score and leverage**.

| Risk Category   | Criteria                             |
| --------------- | ------------------------------------ |
| **High Risk**   | Credit Score < 650 OR DTI > 0.5      |
| **Medium Risk** | Credit Score 650–700 OR moderate DTI |
| **Low Risk**    | Credit Score > 700 AND low DTI       |

This segmentation allows the portfolio to be **monitored by borrower risk level**.

---

### 5. Portfolio Visualization (Power BI)

An interactive **Power BI dashboard** was developed to monitor the portfolio.

Key visuals include:

**KPI Cards**

* Total Borrowers
* High Risk Borrowers
* Total Loan Exposure

**Scatter Plot**

* Credit Score vs Debt-to-Income
* Bubble size represents **Loan Amount**
* Color represents **Risk Category**

**Industry Risk Exposure**

* Stacked bar chart showing risk distribution by industry

**Risk Category Breakdown**

* Pie chart of borrower distribution by risk level

**Interactive Filters**

* Industry
* Risk Category
* Loan Type

A **DAX measure** was created to calculate the number of **High Risk borrowers** dynamically.

---

## 📊 Key Insights

* Borrowers with **DTI above 0.5** tend to fall into the **high-risk segment**
* Lower **credit scores (<650)** significantly increase borrower risk classification
* Some industries show **higher concentrations of high-risk exposure**
* Interactive dashboards allow users to **monitor credit portfolio risk distribution**

---

## 📌 Skills Demonstrated

* Synthetic data generation with Python
* Data cleaning and preprocessing
* Financial ratio analysis (Debt-to-Income)
* Credit risk segmentation
* Data visualization and dashboard development
* DAX measures for portfolio monitoring

---

## 📸 Dashboard Preview

<img width="1293" height="647" alt="image" src="https://github.com/user-attachments/assets/4eb7b98b-48df-4fff-baac-5467d45709d5" />

