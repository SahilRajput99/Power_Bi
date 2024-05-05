# Data Profession Survey Breakdown

### Dashboard Link : https://app.powerbi.com/groups/me/reports/384d017e-e935-44dc-9e7d-1626c1a36de1/ReportSection

## Problem Statment

The dashboard aims to provide insights into the demographics, career paths, and job satisfaction levels of individuals working in the data industry. By analyzing this data, organizations can better understand the needs and preferences of their employees, identify areas for improvement, and make data-driven decisions to enhance employee satisfaction and retention.

## Objective

The objective of this project is to analyze the provided dataset using Power BI to gain insights into the following areas:

- Demographic distribution of data industry employees.
- Career trajectories, including career switches and salary trends.
- Job satisfaction levels across various dimensions.
- Factors influencing career transitions and job preferences within the data industry.

## Steps followed 

### Step 1 : Data Import:

- Load data into Power BI Desktop, dataset is a csv file.

### Step 2 : Data Import:

- Open power query editor & in view tab under Data preview section.
- Removed columns such as Browser, OS, City, Country, and Referrer which were not relevant for analysis.
- It was observed that in none of the columns like "which country do you live in", "which title fits your job role" & " current annual salary" were not in proper format to create visual reports.

### Step 3 : Role and Programming Language Standardization:

- Split the "Which Title Best Suits Your Current Role" and "Favorite Programming Language" columns to standardize responses.
- Created a split column for the "Others" category where respondents specified their job role or programming language.

### Step 4 : Salary Data Standardization:

- Split the "Current Yearly Salary" column as it was in a range format.
- Created an average salary column to represent the rounded average salary value.
- Formatted the data into a cleaner and more user-friendly format.

### Step 5 : Geographical Distribution Standardization:

- Split the "Which Country Do You Live In" column to standardize responses.
- Created a split column for the "Others" category where respondents specified their country

### Step 6 : Data Transformation:

- Applied necessary transformations and data cleaning steps in Power Query Editor.
- Ensured data consistency and accuracy for further analysis.

### Step 7 : Visualization and Dashboard Creation:

- In the report view, under the insert tab, text box was added to the canvas, and the name of the project "Data profession Survery Breakdown" was mentioned
- New measure was created to find total count of Survey.
Following DAX expression was written for the same,
        
        Count of survery = COUNT(Data_professional_survery[ID])
        
A card visual was used to represent count of customers.

![count of people](https://github.com/SahilRajput99/Power_Bi/assets/168499493/2d6a432c-dd21-4e81-a87f-8cfd2a79902a)
      
 - New measure was created to find  Average age of survery people,
 
 Following DAX expression was written to find Average age,
 
         Average Age = Average(Current_age)
 
 A card visual was used to represent the Average Age.

![Average age](https://github.com/SahilRajput99/Power_Bi/assets/168499493/23c74f16-db1a-4ee9-96f6-03c9c3f77a1b)

Following are the charts which I created further.

- Average Salary for Job Title (Stacked Bar Chart):

    Create a measure: "Average Salary by Job Title" using AVERAGE function.

    Add a clustered column chart with job titles on the X-axis and the measure on the Y-axis.

- Average Salary by Gender (Pie Chart):

    Create a measure: "Average Salary by Gender" using AVERAGE function.

    Add a pie chart with gender as the legend and the measure as the value.

- Happiness with Current Salary (Gauge Chart):

    Create a measure: "Happiness with Salary" using AVERAGE function.

    Add a gauge chart with the measure.

- Happiness with Work-Life Balance (Gauge Chart):

    Create a measure: "Happiness with Work-Life Balance" using AVERAGE function.

    Add another gauge chart with the measure.

- Favorite Programming Language (Stacked Column Chart):

    Add a stacked column chart with programming languages on the X-axis and salary on the Y-axis.

- Average Salary by Country (Treemap Chart):

    Create a measure: "Average Salary by Country" using AVERAGE function.
    
    Add a treemap chart with countries grouped and the measure as the value.
 
 - Step 18 : The report was then published to Power BI Service.
 
![Public message](https://github.com/SahilRajput99/Power_Bi/assets/168499493/6fdd2f32-0fd2-4b37-b59c-01d7425ad4dc)


# Snapshot of Dashboard (Power BI Service)

![Dashboard snap](https://github.com/SahilRajput99/Power_Bi/assets/168499493/edc87e7d-0e53-4173-b9a4-62dabc127541)


 # Report Snapshot (Power BI DESKTOP)
![Dashboard snap](https://github.com/SahilRajput99/Power_Bi/assets/168499493/edc87e7d-0e53-4173-b9a4-62dabc127541)

# Insights

A single page report was created on Power BI Desktop & it was then published to Power BI Service.

Following inferences can be drawn from the dashboard;

### Total Number of Survery = 630

###   Job Title vs. Average Salary:

- Data Scientists have the highest average salary at $94.04, followed by Data Engineers and Data Architects.
- Data Analysts and Database Developers have lower average salaries.
- Other roles and students/individuals looking for roles also have significant representation, with average salaries in the mid-range.

### Gender Vs Salary:

- On average, females have a slightly higher average salary compared to males ($55.37 vs. $53.61).
- This indicates a relatively balanced distribution of salary across genders in the surveyed population.

### Age Distribution:

- The average age of survey participants is approximately 29.87 years, indicating a relatively young demographic.

### Salary Satisfaction:

- Participants generally seem satisfied with their current salary, with an average rating of 4.27 out of 10.
- However, there is a range of satisfaction levels, with some respondents indicating very high satisfaction and others indicating dissatisfaction.

### Favorite Programming Languages:

- Python emerges as the most popular programming language among survey respondents, followed by R.
- Other languages and those who identify as students or are looking for roles also show significant representation.

### Geographical Salary Distribution:

- The United States has the highest total sum of average salaries, followed by other countries such as India, Canada, and the United Kingdom.
- This suggests varying salary levels across different geographical regions.

### Work-Life Balance Satisfaction:

- Participants generally report a positive work-life balance, with an average rating of 5.74 out of 10.
- The range of responses indicates that while many are satisfied, there are also those who report lower levels of satisfaction or struggle with work-life balance issues.

---------------------------- End--------------------------
