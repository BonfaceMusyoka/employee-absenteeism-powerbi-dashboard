# 📊 Power BI Project: Employee Absenteeism Behavior and Cost Analysis

---

## 🔺 Executive Summary

This Power BI dashboard analyzes employee absenteeism data to uncover behavioral patterns, cost drivers, and time trends.  
The goal is to empower HR decision-makers to understand **why, when, and how employees are absent**, and what **impact it has on the organization**.

---

## 🔹 Key Insights

- **Smoking behavior is a major driver of absenteeism**  
  Employees who smoke accounted for **4,773 hours** absent, compared to only **351 hours** among non-smokers — over **13x higher**.

- **Social drinking correlates with higher absenteeism**  
  Drinkers missed **3,226 hours**, nearly double the **1,898 hours** recorded by non-drinkers.

- **Absenteeism peaks in March and July**  
  March (**765 hrs**) and July (**734 hrs**) had the highest recorded absences, likely tied to seasonal or health patterns.

- **Cost trends mirror absenteeism peaks**  
  March (**KES 31k**) and July (**KES 28k**) had the highest absenteeism-related costs, highlighting financial implications.

- **Top 5 reasons account for most absentee cases**  
  1. Musculoskeletal diseases  
  2. Injury and poisoning  
  3. Medical consultation  
  4. Dental consultation  
  5. Digestive system diseases

- **Lower-educated employees dominate absentee cases**  
  Among the top 10 most absent employees, **9 had only high school education**, and only **1 had a master's degree**.

---

## ⚙️ Project Details

### 📁 Dataset Overview

The dataset includes three related tables:

| Table Name     | Description |
|----------------|-------------|
| `Absenteeism`  | Main fact table capturing absence events and employee demographics |
| `Reasons`      | Lookup table mapping numeric codes to medical absence reasons |
| `Compensation` | Hourly wage per employee, used to compute absenteeism cost |

---

### 🛠 Tools & Techniques Used

- **Power BI Desktop**: Data modeling, DAX measures, interactive visuals
- **Power Query**: Merges, derived columns, data cleaning
- **Data Relationships**:
  - One-to-many join between `Reasons` and `Absenteeism`
  - One-to-one join between `Compensation` and `Absenteeism`
- **Custom Columns**:
  - `Season Description` (1 = Winter, etc.)
  - `Month Name` (sorted by `Month Number`)
  - `Education Level`
  - `Smoking Status` and `Drinking Status`
- **DAX Measures**:
  - Total Absenteeism Hours
  - Total Absenteeism Cost
  - Average Hours per Employee

---
## 🔍 Dashboard Previews

### 📄 Page 1 – Executive Summary
![Executive Summary](./images/page1.png)

### 📄 Page 2 – Behavioral & Demographic Insights
![Behavioral Insights](images/page2.png)

### 📄 Page 3 – Cost & Trend Analysis
![Cost Analysis](images/page3.png)

