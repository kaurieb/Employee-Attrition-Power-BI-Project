# Human Resources Turnover Rate
## Project Background and Overview 
This analysis explores the root causes of employee attrition using a detailed HR dataset that spans demographics, compensation, departmental roles, performance metrics, and employee satisfaction. By identifying and uncovering patterns among high-risk groups such as early-tenure staff, low earners, specific departments, and underrepresented groups, this project highlights critical areas contributing to turnover. These insights will help HR leadership focus on the most impactful drivers of turnover and inform strategies to reduce attrition. To complement my analysis, an interactive Power BI dashboard visualizes critical metrics, enabling real-time tracking of attrition KPIs and at-risk employee profiles across the organization. 

The following five categories were prioritized for analysis based on their statistically significant correlation with attrition rates in our dataset, as well as their actionable potential for HR leadership to implement data-driven strategy. Hence, in this report, insights and recommendations are provided on the following key areas:

1.	**Gender Disparities** :
   Why? Evaluating gender-based attrition patterns sheds light on turnover risks in the gender demographic. 
2.	**Salary-Driven Attrition** :
   Why? To explore the need for department-specific retention dynamics tied to wages or other possible non-salary factors leading to employee turnover.
3.	**High-Risk Employee Profile** :
   Why? To investigate if there are any employee “hotspots” leading turnover rates within the company. 
4.	**Department-Specific Strategies** :
   Why? To assess if attrition rates varied radically by department, to justify necessitating tailored solutions rather than ‘one-size-fits-all’ policy.
5.	**Proactive Monitoring** :
   Why? To recommend real-time tracking of high-risk groups to HR leadership to enable early intervention, turning reactive attrition management into proactive employee retention.

Click here to go to the dataset used in this project
Click here to go to the interactive Power BI Dashboard 

## Dataset Structure and Overview
![image](https://github.com/user-attachments/assets/cebe0cc0-4cca-41a8-86c7-f2d47a7e47f3)

This Database structure as seen above consists of four relational tables: HR_Data, Education, Jobs and Department, with a total row count of 1,481 records

![image](https://github.com/kaurieb/Power-BI-Project/blob/d054499b33738fe20a3a0e6f425375a4faea1e0f/HR%20dataset%20full%20names.png)

The **HR_Data** table serves as the main dataset, containing detailed employee-level information. Each row represents an individual employee, identified by a unique ID. This table includes demographic details, employment information, and various performance and satisfaction metrics. However, some columns, such as ‘Total Working Years’ and ‘Years At Company’, contain missing values, indicating potential gaps in historical records.

The **Education** table is a simple reference mapping between Education_ID and corresponding fields of study: Life Sciences, Medical, Marketing, Technical Degree, Human Resources and Other. This provides context to the Education values found in the HR_Data table, serving as a distinct record of each educational background represented at the company.

The **Jobs** table links Job_ID with specific job roles: Laboratory Technician, Research Scientist, Sales Representative, Human Resources, Manufacturing Director, Sales Executive, Healthcare Representative, Research Director and Manager, offering clarity for interpreting the JobID in the HR_Data table.

The **Departments** table maps Department_ID to department names: Sales, Research and Development and Human Resources, aiding in the interpretation of department codes in the HR_Data table.

## Executive Summary 
My analysis reveals that attrition is driven by distinct patterns across demographics, employee tenure, and departments. Early-career employees in the age range of 26–35 with ≤ 1 year tenure face the highest turnover risk, highlighting vulnerabilities in onboarding and role alignment. In addition, low compensation is a critical factor in Research Development and HR with 83% of leavers earning ≤5K (the lowest wage bracket), while Sales attrition stems from non-salary issues with 39% of departures being mid-tier earners. Notably, HR exhibits a gender disparity, with female attrition rates doubling the company average for overall female turnover rate (30% vs. 15%). These findings underscore the need for department-specific interventions, with priority given to salary adjustments, early-tenure support, and targeted retention programs for high-risk groups.

Below is the overview page from the interactive Power BI dashboard which can be downloaded here 
![image](https://github.com/kaurieb/Power-BI-Project/blob/f9352d0922c7fc60cf116938046fa199ee0ea43d/whole%20dashboard.png)

## Deep Dive Analysis  
### A.	Gender Analysis
#### Males Drive Overall Attrition, but HR Females Face Disproportionate Risk
#### Company-wide:
- Males (60% of workforce) account for 63% of the company’s attrition (17% attrition rate).
![image]()
- Females (40% of workforce) account for 37% of the company’s attrition (15% attrition rate).
![image]()
- *Takeaway*: The attrition rates in women should take precedence as their population is not represented as highly as the overall male population at the company 

#### HR Department:
- 30% of females in HR left (6 of 20), compared to a 15% average female attrition rate company-wide.
![image]()
- *Implication*: HR females face unique retention challenges (perhaps: workload, advancement opportunities, or cultural misalignment etc. ).

### B.	Salary Impact 
#### Low Pay Drives Turnover in Research and Development & HR, but Sales Tells a Different Story
At first glance, the dashboard shows that 69% of employees who left the company were earners in the salary range of up to 5K which could imply that salary was the main cause of employee attrition. Upon closer analysis at each departmental level, I discovered some interesting finidings.  
#### Research and Development & HR:
- 83% of employees who left cited salaries ≤5K as their reason.
![image]()
- *Takeaway*: Below-market compensation is a critical retention barrier in these departments.
  
#### Sales:
- The department with the highest level of employee attrition with a 21% attrition rate (93 of 450 employees left).
- 36 leavers (39%) earned between 5K–10K, a mid-tier salary range.
- *Implication*: Non-salary factors most likely drove sales employees to leave the company. Perhaps, factors such as: job stress, lack of recognition, or unrealistic targets, likely drive Sales attrition.

### C.	High-Risk Employee Profile: 
#### Young, Low-Tenure, Low-Paid Employees
![image]()
- Age 26–35, salary ≤5K, and 1 year tenure employees had the highest attrition rates across all departments.
- Interpretation: Employees in early career stages are most vulnerable to turnover, likely due to:
- Limited advancement opportunities.
- Mismatch between job expectations and reality.
