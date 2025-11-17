# Customer-Churn-Analysis-...Python-EDA

# 📊 Telco Customer Churn Analysis  
### 🚀 Advanced Data Analytics Project | EDA • Storytelling 
Customer churn is one of the biggest financial challenges in the telecom industry.  
This project is an **end-to-end analytical case study** involving **data cleaning**, **EDA**, **visualization**.

This repository showcases my ability to:
- Handle real-world messy datasets  
- Transform data into insight-heavy stories  
- Communicate insights that directly influence decision-making  
- Think like a **data analyst + business strategist**  
- Present findings professionally for stakeholders  

---

# 🌟 Why This Project Is Valuable

Telecom churn affects:
- Revenue  
- Customer acquisition cost  
- Operational efficiency  
- Customer lifetime value (CLV)  
- Market competitiveness  

Understanding *who* is leaving and *why* helps businesses design effective retention strategies.  
This project approaches churn from **data, customer behavior, and business perspective** → something recruiters love to see.

---

# 🧠 Executive Summary (For Recruiters)

✔ Over **7,000 customer profiles** analyzed  
✔ Identified **6 major churn-driving segments**  
✔ Converted messy raw data into clean analytical dataset  
✔ Developed **actionable business recommendations**  
✔ Delivered insights that solve a real industry problem  
✔ Presented results visually, cleanly, and professionally  

This project reflects **strong analytical thinking**, **problem-solving mindset**, and **business intelligence skills**.
# Dataseet used 
<a href="https://github.com/Kiranbr01/Customer-Churn-Analysis-...Python-EDA-/blob/main/Customer%20Churn.csv">DATASET</a>

---

# 📁 Dataset Overview

The dataset includes:
- **Demographic features** (Gender, SeniorCitizen, Partner, Dependents)  
- **Service subscription info**  
- **Billing & payment details**  
- **Contract type and tenure**  
- **Target variable:** Churn (Yes/No)

📌 **Rows:** 7,043  
📌 **Columns:** 21  
📌 **File:** Telco_Customer_Churn.csv  

---

# 🧼 Data Cleaning & Transformation

### ✔ Missing Value Handling  
`TotalCharges` contained missing and string-formatted numbers. Fixed with type conversion + median imputation.

### ✔ Binary Column Conversion  
Converted numeric indicators → readable categories:

```python
def conv(x):
    return "yes" if x == 1 else "no"
df['SeniorCitizen'] = df['SeniorCitizen'].apply(conv)
