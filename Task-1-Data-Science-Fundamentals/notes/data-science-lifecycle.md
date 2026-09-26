# Day 2 — Data Science Lifecycle & Types of Analysis

## 1. Data Science Lifecycle

A Data Science project generally follows a structured process:

**Problem Definition → Data Collection → Data Cleaning → EDA → Analysis/Modeling → Evaluation → Communication → Deployment/Monitoring**

### Problem Definition
The first step is to clearly understand the problem that needs to be solved. A clear problem statement helps decide what data and analysis are required.

### Data Collection
Relevant data is collected from sources such as databases, APIs, surveys, websites, sensors, company records, CSV/Excel files, or public datasets.

### Data Cleaning
Real-world data may contain missing values, duplicate records, incorrect values, wrong data types, outliers, or inconsistent formatting. These issues should be handled before analysis.

### Exploratory Data Analysis (EDA)
EDA is used to understand the dataset through summaries, statistics, tables, and visualizations. It helps identify patterns, trends, relationships, and unusual observations.

### Statistical Analysis / Modeling
Statistical techniques or Machine Learning models can be used depending on the problem. Examples include mean, median, correlation, hypothesis testing, regression, and classification.

### Evaluation
The results are checked to determine whether the analysis or model is reliable and useful. Machine Learning models may use metrics such as accuracy, precision, recall, and F1-score.

### Communication
Findings should be communicated clearly using simple explanations, charts, reports, or dashboards so that other people can understand the results.

### Deployment and Monitoring
If a model or solution is intended for real-world use, it can be deployed in an application or system. Its performance should then be monitored over time.

---

## 2. Types of Data Analysis

### Descriptive Analysis — What happened?
Descriptive analysis summarizes historical data.

Example: Sales decreased from ₹10 lakh in January to ₹8 lakh in February.

### Diagnostic Analysis — Why did it happen?
Diagnostic analysis investigates the reasons behind an observed result.

Example: Sales decreased because important products were out of stock and website traffic decreased.

### Predictive Analysis — What may happen?
Predictive analysis uses existing or historical data to estimate future outcomes.

Example: Based on previous sales patterns, March sales are estimated to be around ₹9 lakh.

### Prescriptive Analysis — What should we do?
Prescriptive analysis focuses on possible actions based on available insights.

Example: Increase inventory for popular products and improve marketing campaigns.

---

## 3. Easy Memory Trick

- **Descriptive:** What happened?
- **Diagnostic:** Why did it happen?
- **Predictive:** What may happen?
- **Prescriptive:** What should we do?

---

## 4. Example — Student Performance Analysis

Suppose a dataset contains:

- Student ID
- Age
- Gender
- Attendance
- Study Hours
- Marks
- City

### Problem
Understand which factors are associated with student marks.

### Useful Data
Attendance, study hours, marks, age, and other relevant student attributes.

### Possible Cleaning
Check missing values, duplicates, incorrect values, inconsistent categories, and wrong data types.

### EDA
Explore questions such as:
- What are the average marks?
- Is attendance related to marks?
- Are study hours related to marks?
- What is the distribution of marks?

### Visualization
Scatter plots can be useful for exploring relationships such as Study Hours vs Marks or Attendance vs Marks.

### Communication
Summarize the important patterns with supporting statistics and charts, while avoiding claims that the data does not support.

---

## 5. What I Learned Today

Today I learned:
- The main stages of the Data Science lifecycle
- Why defining the problem comes before analysis
- Why data cleaning and EDA are important
- The difference between descriptive, diagnostic, predictive, and prescriptive analysis
- How the lifecycle can be applied to a simple real-world dataset

## Key Takeaway

A good Data Science project is not just about building a model. It starts with understanding the problem and data, then moves through cleaning, exploration, analysis, evaluation, and clear communication.

---

**Day 2 Status: Complete ✅**
