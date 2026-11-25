# HR Attrition Analysis | Microsoft Fabric | Power BI | IBM HR Analytics

An end-to-end HR analytics project using Microsoft Fabric and Power BI to investigate employee attrition, identify workforce trends, and understand the factors associated with employee turnover.

The project uses the IBM HR Analytics Employee Attrition & Performance dataset containing 1,470 employee records. It combines data ingestion, transformation, analytical modeling, interactive dashboard development, and data security implementation.

The solution includes two interactive dashboard pages: **HR Attrition Overview** and **HR Attrition Deep Dive**, supported by conditional formatting, calculated measures, and access-control configurations.

---

## Project Objectives

- Analyze employee attrition across departments and job roles.
- Identify employee groups with higher attrition rates.
- Examine the relationship between salary bands and employee turnover.
- Explore attrition patterns across age groups, gender, education, marital status, business travel, and overtime.
- Implement data access restrictions to protect sensitive employee information.
- Present HR insights through interactive Power BI dashboards.

## Tools & Technologies

| Category | Technologies |
|---|---|
| Data Platform | Microsoft Fabric |
| Data Ingestion | Dataflows Gen2 |
| Data Transformation | Power Query |
| Data Analysis | Power BI |
| Calculations | DAX |
| Data Modeling | Power BI Semantic Model |
| Security | Dynamic RLS, CLS, Sensitivity Labels |
| Dataset | IBM HR Analytics Employee Attrition & Performance |

---

## Project Workflow

### 1. Data Ingestion & Transformation – Microsoft Fabric

- Imported the IBM HR Analytics dataset into Microsoft Fabric.
- Ingested 1,470 employee records using Dataflows Gen2.
- Performed data cleaning and transformation using Power Query.
- Created a custom Salary Band column using conditional column logic.
- Categorized employees based on monthly income into salary groups:
  - Under 3k
  - 3k to 6k
  - 6k to 10k
  - Above 10k

### 2. Data Modeling & Analysis

Prepared the data for reporting and created analytical measures using DAX.

Key analytical metrics include:
- Total Headcount
- Employees Left
- Attrition Rate
- Average Monthly Income
- Average Tenure of Leavers
- Department-wise Attrition
- Job Role-wise Attrition
- Salary Band-wise Attrition

### 3. Power BI Dashboard Development

Developed two interactive dashboard pages with department, gender, and salary band slicers.

#### Dashboard 1: HR Attrition Overview

The Overview page provides a consolidated view of workforce attrition.

**Key components:**
- Attrition Rate
- Total Headcount
- Employees Left
- Average Monthly Income
- Average Tenure of Leavers
- Overall Attrition Composition
- Attrition by Department
- Attrition Decomposition
- Attrition by Job Role
- Attrition by Age Group

#### Dashboard 2: HR Attrition Deep Dive

The Deep Dive page explores employee attrition across additional workforce characteristics.

**Key components:**
- Attrition by Marital Status
- Attrition by Education Field
- Attrition by Gender
- Attrition by Overtime
- Attrition by Business Travel

Both pages include interactive filtering to explore different employee segments.

### 4. Data Security & Governance

Implemented data protection and access-control features in the project.

**Dynamic Row-Level Security (RLS)**
- Implemented dynamic access control using DAX and User Principal Name (UPN).
- Configured department-based access so department heads can view their respective department's employee data.

**Column-Level Security (CLS)**
- Implemented column-level access restrictions to protect selected sensitive employee information.

**Sensitivity Labels**
- Applied a Confidential sensitivity label to support the protection of employee-related information.

### 5. Conditional Formatting & Data Transformation

Additional implementation work included:

- Created custom Salary Band categories using conditional columns in Power Query.
- Applied conditional formatting in Power BI Matrix visuals.
- Used colour-based formatting to highlight attrition percentages.
- Used data bars to improve comparisons across job roles.
- Designed visual indicators to make higher-attrition employee groups easier to identify.

---

## Key Dashboard Metrics

The following figures are taken from the latest Overview dashboard.

| Metric | Result |
|---|---:|
| Total Headcount | 1,470 |
| Employees Left | 237 |
| Overall Attrition Rate | 16.12% |
| Average Monthly Income | 6,503 |
| Average Tenure of Leavers | 5.1 Years |

## Key Business Insights

### 1. Department-wise Attrition

| Department | Attrition Rate |
|---|---:|
| Sales | 20.63% |
| Human Resources | 19.05% |
| Research & Development | 13.84% |

Sales recorded the highest attrition rate among the three departments.

### 2. Job Role-wise Attrition

Sales Representatives recorded an attrition rate of approximately 39.76%, making this one of the highest-attrition job roles in the analysis.

### 3. Age Group Analysis

| Age Group | Headcount | Employees Left | Attrition Rate |
|---|---:|---:|---:|
| 18 to 25 | 123 | 44 | 35.77% |
| 25 to 35 | 606 | 116 | 19.14% |
| 45 to 60 | 273 | 34 | 12.45% |
| 35 to 45 | 468 | 43 | 9.19% |

The 18–25 age group recorded the highest attrition rate.

### 4. Gender Analysis

| Gender | Attrition Rate |
|---|---:|
| Male | 17.01% |
| Female | 14.80% |

Male employees recorded a higher attrition rate than female employees.

### 5. Marital Status Analysis

| Marital Status | Attrition Rate |
|---|---:|
| Single | 25.5% |
| Married | 12.5% |
| Divorced | 10.1% |

Single employees recorded the highest attrition rate among the three marital-status categories.

### 6. Business Travel Analysis

| Business Travel | Attrition Rate |
|---|---:|
| Travel Frequently | 24.91% |
| Travel Rarely | 14.96% |
| Non-Travel | 8.00% |

Employees who travelled frequently showed a higher attrition rate.

### 7. Overtime Analysis

| Overtime | Attrition Rate |
|---|---:|
| Yes | 30.53% |
| No | 10.44% |

Employees working overtime recorded a substantially higher attrition rate than employees who did not work overtime.

### 8. Education Field Analysis

| Education Field | Attrition Rate |
|---|---:|
| Human Resources | 25.93% |
| Technical Degree | 24.24% |
| Marketing | 22.01% |
| Life Sciences | 14.69% |
| Medical | 13.58% |
| Other | 13.41% |

Human Resources recorded the highest attrition rate among the education fields shown.

---

## Dashboard Screenshots

### 1. HR Attrition Overview

Provides a consolidated view of workforce metrics, department-wise attrition, job roles, age groups, and attrition decomposition.

<img width="1532" height="728" alt="HR Attrition Overview Dashboard" src="https://github.com/user-attachments/assets/e3616c7b-fc31-421d-9e12-8264386e636f" />

### 2. HR Attrition Deep Dive

Explores employee attrition patterns across marital status, education field, gender, overtime, and business travel.

<img width="1532" height="722" alt="HR Attrition Deep Dive Dashboard" src="https://github.com/user-attachments/assets/65fda582-1f75-412f-8560-8453f9b302d7" />

### 3. Salary Band Creation – Conditional Column

Demonstrates the creation of custom salary categories using conditional column functionality in Microsoft Fabric Power Query.

<img width="1535" height="727" alt="Salary Band Conditional Column" src="https://github.com/user-attachments/assets/b46c505a-c23d-4dbb-acab-f43011787204" />

### 4. Data Security Implementation – RLS & CLS

Demonstrates the data security implementation for controlling access to employee information.

<img width="1535" height="726" alt="HR Data Security Implementation" src="https://github.com/user-attachments/assets/1945a1e9-368d-4c9e-835b-64ab3bd7727b" />

---

## Skills Demonstrated

- Microsoft Fabric
- Dataflows Gen2
- Power Query
- Data Cleaning & Transformation
- Conditional Column Creation
- Power BI Dashboard Development
- DAX Measures
- Interactive Data Visualization
- Matrix Conditional Formatting
- Data Modeling
- Dynamic Row-Level Security (RLS)
- Column-Level Security (CLS)
- Sensitivity Labels
- HR Analytics
- Business Intelligence
- Data-Driven Decision Making

---

## Business Value

This project demonstrates how HR analytics can help organizations understand employee turnover, identify workforce segments with higher attrition, and investigate potential retention challenges.

By combining Microsoft Fabric data preparation, Power BI analytics, and security configurations, the solution provides an interactive and structured approach to workforce analysis.

---

**Dataset:** IBM HR Analytics Employee Attrition & Performance

**Platform:** Microsoft Fabric & Power BI

**Project Type:** End-to-End HR Data Analytics
