# 💼 Credit Risk Portfolio Analysis

This mini project performs an **end-to-end analysis of SME loan portfolios** to identify high-risk borrowers, assess portfolio exposure, and showcase actionable insights for risk management.

---

## 🛠 Tools & Technologies

- **Python**: Pandas, Numpy and Matplotlib for data generation,cleaning and analysis  
- **Power BI**: Interactive dashboards and visualization  
- **Excel**: Initial exploration on CSV file 

---

## 🔍 Project Overview

The project involves:  

1. **Data Generation**
   - Randomly generate loan portfolio data, including:  
     - Borrower_ID  
     - Industry  
     - Loan_Amount  
     - Revenue  
     - Credit_Score  
   - Ensures reproducible example data for testing  

2. **Data Cleaning & Preparation**
   - Remove duplicate borrower records  
   - Standardize text fields (e.g., Industry names)  
   - Handle numeric issues (e.g., zero or negative revenue)  

3. **Debt-to-Income (DTI) Calculation**
   - Calculate `Debt_to_Income = Loan_Amount / Revenue`  
   - Flag high-leverage borrowers  

4. **Risk Category Assignment**
   - **High Risk**: Credit Score < 650 OR DTI > 0.5  
   - **Medium Risk**: Credit Score 650–700 OR moderate DTI  
   - **Low Risk**: Credit Score > 700 AND low DTI  

5. **Portfolio Summary**
   - Aggregate metrics by Industry and Risk Category  
   - Generate summary tables for dashboard visualization  

6. **Data Visualization**
   - KPI Cards: Total borrowers, high-risk count, total loan exposure  
   - Scatter plot: Credit Score vs DTI (bubble size = Loan Amount, color = Risk Category)  
   - Industry-level risk exposure: stacked bar charts
   - Risk Category breakdown: Pie Chart
   - Interactive slicers: Industry, Loan Type, Risk Category  

---

## 📊 Key Insights

- High-risk borrowers are concentrated where **Debt-to-Income > 0.5** or **Credit Score < 650**  
- Certain industries, e.g., **Service**, have higher high-risk exposure  
- Portfolio dashboards allow **interactive monitoring of high-risk clusters** for decision making  


