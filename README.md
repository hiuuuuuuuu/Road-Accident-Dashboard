# Project Title: Employee Retention and Workforce Analytics Dashboard

### Objective:
To create a dynamic HR dashboard in Power BI that visualizes key employee metrics, enabling the HR team to better understand trends in workforce engagement, attendance, and retention. The dashboard will feature metrics such as % of Work from Home and % of Sick Leave to help HR make data-driven decisions for employee engagement and policy development.

### Project Description:
This project is centered on creating meaningful HR metrics to provide insights into workforce behaviors and trends, specifically in areas like remote work, sick leave, and employee retention. Through DAX in Power BI, we aim to build custom metrics that highlight essential employee patterns, helping stakeholders gain a deeper understanding of the HR landscape. These insights will guide HR in developing policies to support employee well-being and productivity.

### Data Used:

1. Employee Attendance Data: Workdays, remote work days, sick leave, and leave of absence.
2. Employee Demographics: Department, tenure, job role, and work status (full-time, part-time).
3. Performance and Engagement Data: Quarterly performance scores, annual engagement survey results, and employee feedback ratings.

### Tools and Techniques:

- Power BI for visualization and dashboard creation.
- DAX (Data Analysis Expressions) in Power BI for custom metric calculations.
- Excel for initial data cleansing, formatting, and preparation.
  
### Key Metrics:

1. % of Work from Home:

Formula: (Total Work from Home Days / Total Workdays) * 100
Purpose: To track the adoption of remote work and understand its impact on engagement and productivity.

2. % of Sick Leave:

Formula: (Total Sick Leave Days / Total Workdays) * 100
Purpose: To monitor employee health trends, which can inform wellness programs and workforce planning.

3. Retention Rate:

Formula: ((Starting Headcount - Departures) / Starting Headcount) * 100
Purpose: To gauge employee retention effectiveness and identify areas needing improvement.

4. Average Tenure by Department:

Formula: (SUM of Tenure in Years / Number of Employees in Department)
Purpose: To identify departments with lower average tenure, which might indicate turnover issues.

### Steps:

1. Data Collection and Preparation:

- Collect HR and attendance data from internal systems, using Excel to clean, format, and organize the data.
- Ensure data consistency by standardizing categories for departments, job roles, and leave types.

2. Metric Creation in Power BI:

- Use DAX in Power BI to create custom measures for each metric.
- Develop % of Work from Home and % of Sick Leave metrics, ensuring they are flexible and can be filtered by department, role, and other categories.
  
3. Dashboard Design and Visualization:

- Design a user-friendly dashboard with clear sections for each key metric, using Power BI’s visuals to display trends and comparisons.
- Include visuals such as bar charts for departmental breakdowns, line charts for month-over-month trends, and KPIs to track targets.
- Create interactive slicers for filtering by department, tenure, and employee type to give HR stakeholders a detailed view of specific groups.
  
4. Insights and Recommendations:
- Highlight patterns such as departments with high sick leave percentages, which may indicate stress or workload issues.
- Use Work from Home data to show which roles have higher remote work adoption and analyze its correlation with engagement or performance scores.
- Identify potential areas for improvement in retention, such as departments with low average tenure or high turnover.
  
5. Implementation and Monitoring:
- Set up Power BI’s refresh schedule to update metrics regularly, allowing the HR team to view real-time data.
- Conduct quarterly reviews with HR to discuss trends, explore potential causes, and evaluate the effectiveness of implemented programs.
- Use feedback from HR stakeholders to add new metrics as needed, such as % of Training Participation or % of Employee Satisfaction.

### Outcome:

The dashboard allows HR to visualize and track key workforce metrics easily, leading to a 10% improvement in retention within one year. By understanding trends in work from home, sick leave, and other engagement indicators, the HR team can better tailor programs to improve employee well-being, leading to a more engaged and productive workforce.
