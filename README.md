# Project Title: Employee Leave Tracking and Time-Off Analysis Dashboard

### Objective:
To provide a comprehensive analysis of employee leave usage, including various leave categories, to help HR monitor trends and ensure policy compliance. This dashboard will track both full-day and half-day leave usage across different leave types such as paid leave, sick leave, work from home, etc.

ask :  the working preference of people: work from home or work from office.

### Key Leave Categories:

- Paid Leave (PL)
- Sick Leave (SL)
- Half Day Paid Leave (Half PL)
- Half Day Sick Leave (Half SL)
- Work from Home (WFH)
- Floating Festival Leave
- Half Day Floating Festival Leave
- Birthday Leave
- Leave Without Pay (LWOP)
- Half Day Leave Without Pay
- Bereavement Leave
- Half Bereavement Leave
- Half Work from Home
- Weekly Off
- Holiday Off
- Menstrual Leave (ML)
- Half Day Menstrual Leave (Half ML)


### Tools and Techniques:

- Excel: For data preparation, cleaning, and initial calculations.
- Power BI: For building interactive dashboards and visualizations.
- DAX: For creating custom metrics in Power BI (e.g., leave usage percentage, trends).
  

### Steps:

#### 1. Data Collection and Preparation:

1. Gather employee leave data (e.g., Excel or from HR systems) that includes:
- The type of leave (Paid Leave, Sick Leave, Work from Home, etc.).
- The duration of the leave (full-day or half-day).
- Dates of leave and any special notes (e.g., for floating holidays or bereavement leave).
2. Clean the data in Excel:
- Ensure all data is consistent (e.g., proper leave type names, uniform date formats).
- Calculate the total leave days for each employee (e.g., for half-day leaves, mark the value as 0.5).

#### 2. Data Modeling in Power BI
1. Import the leave data and employee data into Power BI.

2. Create relationships between tables (e.g., linking employee data with leave data using employee IDs).

3. Develop calculated columns and measures in DAX for specific leave types:

- Total Paid Leave (PL):
Total Paid Leave = CALCULATE(SUM(LeaveData[Leave Duration]), LeaveData[Leave Type] = "PL")
- Total Sick Leave (SL):
Total Sick Leave = CALCULATE(SUM(LeaveData[Leave Duration]), LeaveData[Leave Type] = "SL")
- Total Work from Home (WFH):
Total Work from Home = CALCULATE(SUM(LeaveData[Leave Duration]), LeaveData[Leave Type] = "WFH")
- Total Leave by Type:
Total Leave by Type = CALCULATE(SUM(LeaveData[Leave Duration]))

4. Create additional calculated fields to handle half-day leaves:
- Half Day Paid Leave:
Half Day Paid Leave = CALCULATE(SUM(LeaveData[Leave Duration]), LeaveData[Leave Type] = "Half PL")
- Half Day Sick Leave:
Half Day Sick Leave = CALCULATE(SUM(LeaveData[Leave Duration]), LeaveData[Leave Type] = "Half SL")
  
#### Dashboard Development in Power BI
1. Leave Summary Dashboard:

Display a pie chart or bar chart showing the percentage distribution of each leave type (e.g., Paid Leave, Sick Leave, Work from Home).
2. Leave Usage Over Time:

Create a line chart that shows leave trends over the months or quarters for each leave type.
Use slicers for filtering by department, employee, or time period.
3. Leave Usage by Department:

Use a stacked bar chart to compare leave usage across different departments, showing which departments are using the most leave.
4. Leave Balance Tracker:

Show the remaining leave balance for each employee or department with KPI indicators.
5. Leave Analysis by Type:

Use tree maps or heatmaps to show patterns of leave usage, focusing on categories like Half Day Paid Leave or Sick Leave.
6. Interactive Slicers:

Allow HR managers to filter the dashboard by employee ID, department, leave type, or leave duration.

#### Advanced Analysis with DAX
Leave Utilization Rate:
Calculate the percentage of total leave usage for each employee or department:

DAX
Sao chép mã
Leave Utilization % = DIVIDE(SUM(LeaveData[Leave Duration]), [Total Leave Duration], 0)
Leave Type Comparison:
Compare the total leave days used for each type across different departments or teams:

DAX
Sao chép mã
Total Leave by Type = CALCULATE(SUM(LeaveData[Leave Duration]), LeaveData[Leave Type] = "PL")
Trend Analysis for Leave:
Create trendlines to track leave usage patterns over time. This can help in understanding seasonal trends or periods of high absenteeism.

#### Insights and Recommendations
1. Identify High Absenteeism:
Use the dashboard to spot employees or departments with high leave usage, especially frequent sick leaves or work from home. This may indicate potential burnout, health issues, or workflow inefficiencies.

2. Optimize Leave Policies:
Based on trends in leave usage, HR can adjust policies, such as offering more floating holidays during peak times or revising sick leave policies.

3. Improve Workforce Planning:
Analyze the correlation between leave usage and productivity to identify optimal staffing levels during high leave periods.

### Outcome:

By completing this project, HR will have a clear, interactive dashboard that allows for:

- Real-time tracking of employee leave.
- Detailed analysis of leave types, including trends, half-day leave, and usage patterns.
- Actionable insights that help HR optimize policies, reduce absenteeism, and improve workforce management.
