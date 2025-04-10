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

The HR_Data table serves as the main dataset, containing detailed employee-level information. Each row represents an individual employee, identified by a unique. This table includes demographic details, employment information, and various performance and satisfaction metrics. However, some columns, such as ‘Total Working Years’ and ‘Years At Company’, contain missing values, indicating potential gaps in historical records.

The Education table is a simple reference mapping between Education_ID and corresponding fields of study: Life Sciences, Medical, Marketing, Technical Degree, Human Resources and Other. This provides context to the Education values found in the HR_Data table, serving as a distinct record of each educational background represented at the company.

The Jobs table links Job_ID with specific job roles: Laboratory Technician, Research Scientist, Sales Representative, Human Resources, Manufacturing Director, Sales Executive, Healthcare Representative, Research Director and Manager, offering clarity for interpreting the JobID in the HR_Data table.

The Departments table maps Department_ID to department names (e.g., Sales, Human Resources), aiding in the interpretation of department codes in the HR_Data table.

