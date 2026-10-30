# HR Attrition Analysis | IBM Dataset | Microsoft Fabric & Power BI

## 📌 Project Overview

This project focuses on analyzing employee attrition using the IBM HR Analytics Employee Attrition & Performance dataset. The objective is to identify the key factors influencing employee turnover and provide actionable insights through an interactive Power BI dashboard.

Built an end-to-end HR analytics solution using **Microsoft Fabric and Power BI**, processing 1,470 employee records through Dataflows Gen2 and uncovering attrition patterns across departments, job roles, salary bands, age groups, and other employee attributes.

The project also incorporates data security practices to ensure sensitive employee information is appropriately protected.

## 🛠️ Tools & Technologies

* **Microsoft Fabric** – Data ingestion and transformation.
* **Dataflows Gen2** – Data preparation and transformation.
* **Power Query** – Data cleaning and conditional column creation.
* **Power BI** – Interactive dashboard development and visualization.
* **DAX** – Calculated measures and dynamic Row-Level Security.
* **UPN (User Principal Name)** – User-based access control.
* **Sensitivity Labels** – Confidential data protection.
* **IBM HR Analytics Dataset** – Employee attrition analysis.

## 📂 Project Workflow

### 1. Data Ingestion & Transformation

* Imported the IBM HR Analytics dataset into Microsoft Fabric.
* Ingested 1,470 employee records using Dataflows Gen2.
* Used Power Query to clean, transform, and prepare the dataset.
* Created a custom **Salary Band** conditional column based on monthly income:

  * Under 3k
  * 3k to 6k
  * 6k to 10k
  * Above 10k

### 2. Data Analysis & Dashboard Development

Developed interactive Power BI dashboards to explore employee attrition patterns.

**Dashboard 1 – HR Attrition Overview**

* Overall attrition rate and employee headcount.
* Total employees who left the organization.
* Average monthly income.
* Average tenure of employees who left.
* Department-wise attrition analysis.
* Attrition decomposition by department, job role, and salary band.
* Job role and salary band comparisons.

**Dashboard 2 – HR Attrition Deep Dive**

* Age-group-wise attrition analysis.
* Gender-based attrition comparison.
* Education-field analysis.
* Marital-status analysis.
* Business-travel impact on attrition.
* Overtime-related attrition analysis.
* Interactive department, gender, and salary-band filters.

### 3. Data Security & Access Control

Implemented security measures to protect employee information:

* **Dynamic Row-Level Security (RLS):** Implemented dynamic access using DAX and User Principal Name (UPN), ensuring department heads can view only their respective department's employee data.
* **Column-Level Data Protection:** Applied column-level access restrictions to protect selected sensitive information.
* **Sensitivity Label:** Applied a Confidential sensitivity label to help protect personal employee data.

## 📊 Key Business Insights

The analysis identified several important attrition patterns:

| Metric                    |   Finding |
| ------------------------- | --------: |
| Total Employees           |     1,470 |
| Employees Left            |       237 |
| Overall Attrition Rate    |     16.1% |
| Average Monthly Income    |     6,503 |
| Average Tenure of Leavers | 5.1 Years |

**Key Observations:**

1. **Department:** Sales recorded the highest attrition rate at 20.6%, followed by Human Resources at 19.0%.

2. **Salary:** Employees earning under 3k had the highest attrition rate at 28.6%, indicating a relationship between lower salary bands and employee turnover.

3. **Job Role:** Sales Representatives recorded a particularly high attrition rate of 39.8%.

4. **Business Travel:** Employees who travelled frequently showed a 33.3% attrition rate in the deep-dive analysis.

5. **Overtime:** Employees working overtime showed a 37.5% attrition rate compared with 13.8% for employees who did not work overtime.

These findings help identify employee groups with higher attrition and highlight areas where HR teams may investigate retention strategies.

## 📸 Project Screenshots

### 1. HR Attrition Overview Dashboard

<img width="1500" height="1049" alt="HR Attrition Analytics Dashboard" src="https://github.com/user-attachments/assets/2f50e764-4090-49db-9f9a-d1189ccb984e" />


### 2. HR Attrition Deep Dive Dashboard

<img width="1518" height="1036" alt="dashboard 2" src="https://github.com/user-attachments/assets/3da01cba-dd75-4543-a77d-b7df722c8dca" />


### 3. Salary Band Creation – Conditional Column in Microsoft Fabric

<img width="1681" height="935" alt="conditional clm" src="https://github.com/user-attachments/assets/6a5bc71c-a4a2-4286-9aad-0a60eeca594c" />


### 4. Data Security Implementation

<img width="1535" height="862" alt="WhatsApp Image 2026-10-30 at 6 53 29 PM" src="https://github.com/user-attachments/assets/87b7d9c5-d3e3-41c1-9c74-6d29af8c7a22" />


## 🎯 Business Objective

The primary objective is to help HR teams understand employee turnover, identify high-risk employee segments, and make data-driven decisions to improve employee retention.

## 💡 Skills Demonstrated

* End-to-End Data Analytics
* Data Ingestion & Transformation
* Microsoft Fabric – Dataflows Gen2
* Power Query & Data Cleaning
* Conditional Column Creation
* Power BI Dashboard Development
* DAX & Dynamic Row-Level Security
* User-Based Access Control
* Data Confidentiality & Security
* Business Intelligence & Data Visualization
* HR Analytics & Business Insights

---

**Dataset:** IBM HR Analytics Employee Attrition & Performance

