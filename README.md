# E-Learning Analytics & Student Dropout Risk Dashboard

An interactive Power BI project for exploring student performance, learning engagement, dropout-risk indicators, and academic alerts.

---

## Table of Contents

- [Project Overview](#project-overview)
- [Business Objectives](#business-objectives)
- [Dashboard Pages](#dashboard-pages)
  - [Student Performance & Engagement](#1-student-performance--engagement)
  - [Dropout Risk & Alerts](#2-student-dropout-risk--alerts)
- [Dataset Overview](#dataset-overview)
- [Data Model & Analysis](#data-model--analysis)
- [Key Metrics](#key-metrics)
- [Power BI Features](#power-bi-features)
- [Business Questions](#business-questions)
- [Business Value](#business-value)
- [Technology Stack](#technology-stack)
- [Repository Structure](#repository-structure)
- [Getting Started](#getting-started)
- [Limitations & Scope](#limitations--scope)
- [Future Improvements](#future-improvements)
- [Author](#author)

---

## Project Overview

The **E-Learning Analytics & Student Dropout Risk Dashboard** is an interactive business intelligence solution built in Microsoft Power BI. It brings together student, academic, dropout-prediction, alert, and system-performance data to support exploration of academic outcomes and student engagement.

The project combines six Excel datasets containing **3,000 records in total**. Its two report pages focus on:

1. Student academic performance and learning engagement.
2. Student dropout-risk indicators and alert trends.

The dashboard is designed to help users move beyond isolated totals and explore patterns across students, programs, courses, academic periods, and alert categories.

## Business Objectives

- Analyze academic performance across programs, courses, and semesters.
- Explore the relationship between attendance, GPA, and LMS engagement.
- Review student enrollment and academic-status distributions.
- Identify students marked as potential dropout risks in the supplied data.
- Examine alert categories and resolution status.
- Provide interactive reporting for academic monitoring and decision support.

---

## Dashboard Pages

### 1. Executive Overview

### 2. Student Performance & Engagement

This page focuses on academic outcomes and student learning behavior.

**Visuals and analysis include:**

- Student attendance versus GPA distribution.
- LMS engagement versus GPA analysis.
- Average GPA by academic program.
- Course-wise academic performance.
- Student enrollment and course distribution.

**Purpose:** Explore how attendance and learning engagement vary alongside academic performance, and compare outcomes across programs and courses.




### 2. Student Dropout Risk & Alerts

This page focuses on students flagged as potential dropout risks, academic-status distribution, and alert monitoring.

**Visuals and analysis include:**

- Student distribution by academic status.
- At-risk student distribution by program.
- Alerts by trigger type and resolution status.
- Attendance and LMS engagement analysis.
- Student-level academic and risk overview.

**Interactive filters include:**

- Academic year
- Semester
- Program
- Student status
- Dropout prediction (Y/N)

**Purpose:** Examine the indicators associated with students flagged as at risk and monitor alerts that may require academic follow-up.



---

## Dataset Overview

The project uses six Excel datasets, each reported as containing 500 records.

| Dataset              |   Records | Contents                                                                  |
| -------------------- | --------: | ------------------------------------------------------------------------- |
| `Student_Info`       |       500 | Student information, programs, enrollment dates, and status               |
| `Academic_Records`   |       500 | Course marks, GPA, attendance, and semester information                   |
| `Academic_Year`      |       500 | Academic year, program, and semester information                          |
| `Dropout_Prediction` |       500 | Attendance, GPA, LMS engagement, financial status, and dropout-risk flags |
| `Alerts`             |       500 | Student alerts, trigger categories, descriptions, and resolution status   |
| `System_Performance` |       500 | CPU usage, memory usage, processed data, and uptime metrics               |
| **Total**            | **3,000** | **Six datasets**                                                          |


## Data Model & Analysis

The datasets are connected through shared identifiers, including `Student_ID`, where applicable.

The modeling and preparation work described for this project includes:

- Importing and organizing the six Excel tables in Power BI.
- Establishing relationships between student information and related academic or operational records.
- Reviewing relationship cardinality and cross-filter direction.
- Checking data types and aggregation behavior.
- Using grouping and aggregation to support student-level and program-level reporting.
- Enabling report visuals to respond to relevant filters.

Relationship cardinality should be based on actual key uniqueness in each table. A one-to-one or one-to-many relationship should not be assumed without checking the underlying records.

## Key Metrics

The report includes or is designed around the following KPI areas:

| Metric                     | What it communicates                                     |
| -------------------------- | -------------------------------------------------------- |
| Total Students             | Student population represented in the report             |
| Average GPA                | Overall academic performance                             |
| Average Attendance         | Attendance level across the selected data                |
| Average LMS Engagement     | Learning-platform engagement level                       |
| Predicted At-Risk Students | Students flagged in the supplied dropout-prediction data |
| Graduated Students         | Number of students with graduated status                 |
| Total Alerts               | Number of student alerts                                 |
| At-Risk Percentage         | Share of students flagged as at risk                     |


## Power BI Features

### Data preparation and modeling

- Excel data import and Power Query preparation.
- Table relationships through shared identifiers.
- Data-type and aggregation checks.

### Measures and reporting

- DAX measures for KPI reporting.
- Aggregated views by student, program, course, and academic period.
- KPI cards for summary indicators.

### Visualizations and interaction

- Scatter charts for relationship analysis.
- Bar and column charts for category comparisons.
- Donut charts for distribution analysis.
- Tables for student-level details.
- Slicers and cross-filtering for interactive exploration.
- Bookmark-based filter panel with open/close behavior.
- Selection-pane and layer management for visual overlays.
- Consistent visual formatting, titles, and colors.

---

## Business Questions

The dashboard supports investigation of questions such as:

1. How does student attendance vary with GPA?
2. Does LMS engagement show a relationship with academic performance?
3. Which programs have more students flagged as potential dropout risks?
4. How are students distributed across active, graduated, and dropped statuses?
5. Which alert categories generate the most alerts?
6. What proportion of alerts are pending versus resolved?
7. How do attendance and GPA compare for students flagged as at risk?
8. How does academic performance differ across courses and programs?

## Business Value

The dashboard provides a centralized reporting view that can help academic teams:

- Monitor student performance and engagement.
- Explore potential academic-risk patterns.
- Identify students who may need closer review.
- Track alert volume and resolution status.
- Compare outcomes across programs and courses.
- Support more informed academic planning and intervention discussions.


## Technology Stack

| Technology          | Role                                      |
| ------------------- | ----------------------------------------- |
| Microsoft Power BI  | Dashboard development and visualization   |
| Power Query         | Data import and transformation            |
| DAX                 | Measures and KPI calculations             |
| Microsoft Excel     | Source datasets                           |
| Power BI Data Model | Table relationships and filtering         |
| GitHub              | Version control and project documentation |

## Repository Structure

```text
E-Learning-Analytics-Dashboard/
│
├── Data/
│   ├── Student_Info.xlsx
│   ├── Academic_Records.xlsx
│   ├── Academic_Year.xlsx
│   ├── Dropout_Prediction.xlsx
│   ├── Alerts.xlsx
│   └── System_Performance.xlsx
│
├── Dashboard/
│   └── E-learning Dashboard.pbix
│
├── Screenshots/
|   ├── Executive Overview.png
│   ├── Student_Performance.png
│   └── Dropout_Risk_Analytics.png
│
└── README.md
```

## Getting Started

1. **Clone the repository.**

   Replace `YOUR-USERNAME` with your GitHub username:

   ```bash
   git clone https://github.com/KashishPundir/E-Learning-Analytics-Dashboard.git
   ```

2. **Open the project folder** on your computer.

3. **Install Power BI Desktop** if it is not already installed:
   [Download Microsoft Power BI Desktop](https://www.microsoft.com/en-us/power-platform/products/power-bi/desktop).

4. **Open the `.pbix` file.** 

5. **Check the data-source paths** in Power Query. If the Excel files are stored in a different location, update the source paths.

6. **Refresh the data** and confirm that the tables and visuals load correctly.

7. **Explore the report** using the slicers, filters, and visual interactions.

---

## Author

**Kashish Pundir**
B.Tech — Computer Science & Engineering (Data Science)

**Areas of interest:** Data Analytics · Business Intelligence · Data Science · Machine Learning

---

Turning student data into meaningful academic insights.

If you find this project useful, consider giving the repository a star.
