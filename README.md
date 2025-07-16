#  IBM HR Dashboard – Tableau Project

##  Objective

The objective of this project is to design and develop an interactive Tableau dashboard that analyzes IBM HR employee data to uncover critical insights related to attrition, satisfaction, demographics, and departmental trends. The goal is to enable HR professionals to make informed, data-driven decisions to improve employee retention and workforce planning.

---

##  Dataset Used

- **Dataset**: IBM HR Analytics Employee Attrition & Performance
- **Format**: CSV
- **Source**: [Kaggle Dataset](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset)

---

##  Questions (KPIs)

### 1. What is the main objective of your IBM HR Tableau project?
To visualize HR data for discovering attrition trends and optimizing HR policies based on job roles, departments, and employee satisfaction.

### 2. Which data sources did you use, and how did you import them into Tableau?
CSV dataset was imported directly into Tableau Desktop using built-in connectors. Data was cleaned using Tableau Prep.

### 3. Can you explain the key KPIs you calculated in this project?
- Attrition Rate  
- Average Monthly Income  
- Years at Company  
- Satisfaction Score  
- Turnover by Department & Role  
- Gender and Education Distribution  

### 4. How is your data model structured? What relationships exist among the tables?
Used a flat file model with a single table. Dimensions (e.g., Department, Gender) and measures (e.g., Income, YearsAtCompany) were visualized without joins.

### 5. Which calculated fields or functions did you create, and what purpose do they serve?
- `AttritionFlag`: IF [Attrition] = 'Yes' THEN 1 ELSE 0  
- `Attrition Rate`: SUM([AttritionFlag]) / COUNT([EmployeeNumber])  
- `Years Group`: Group employees into tenure buckets  
- `Satisfaction Category`: Classify JobSatisfaction into High/Medium/Low  

### 6. What visuals did you use on your dashboard, and why?
- KPI Cards for key HR metrics  
- Bar Charts for department-wise attrition  
- Pie Charts for gender and education breakdown  
- Heatmaps to show attrition risk combinations  
- Filters for dynamic analysis  

### 7. Did you implement filters or slicers?
Yes. Filters include:
- Department  
- Job Role  
- Gender  
- Age Group  
- Education  
- Marital Status  

### 8. How did you handle missing or inconsistent data?
Used Tableau Prep to:
- Remove rows with nulls in critical fields  
- Normalize text categories (e.g., job roles)  
- Validate numerical ranges  

### 9. What insights did you discover?
- High attrition in Sales and HR departments  
- Low-income and low-tenure employees more likely to leave  
- Higher satisfaction correlated with lower attrition  
- Technical roles had higher retention rates  

### 10. How did you publish and share your Tableau report?
Published to **Tableau Public** and shared internally through **Tableau Server** for HR teams and executive leadership.

---

## 📈 Dashboard Screenshot

<img width="2374" height="1624" alt="Dashboard 1 (1)" src="https://github.com/user-attachments/assets/5a6fceee-8f50-4fbf-9d40-55cd5586d3ea" />


---

##  Project Process Summary

- Imported CSV into Tableau  
- Cleaned and transformed with Tableau Prep  
- Built calculated fields for KPIs  
- Designed visuals and filters for interactivity  
- Published to Tableau Public/Server  

---

##  Final Conclusion

The IBM HR Tableau Dashboard transforms employee data into strategic insights for HR professionals. It helps track attrition patterns, assess employee satisfaction, and identify areas for retention improvement — enabling data-backed decisions for a more stable workforce.

---

## 📎 Links

- 🔗 **Dataset**: [Kaggle - IBM HR Dataset](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset)
- 🔗 **Live Tableau Dashboard**: *Coming Soon or Add Your Link Here*
