# PwC Switzerland Power BI Job Simulation
During this job simulation, I enhanced my Power BI skills and demonstrated my ability to understand client needs for data visualization. Below are the key objectives achieved

## Objectives achieved

#### 1. Strengthned PowerBI Skills

- Loaded and cleaned datasets in Power BI Desktop.
- Created multiple visuals to convey key performance indicators (KPIs) and insights effectively.

#### 2. Expertise in Data Visualization

- Designed and developed Power BI dashboards that showcased KPIs.
- Utilized a variety of visuals including bar charts, slicers, and card visuals to represent data clearly.

#### 3. Effective Communication

- Demonstrated strong communication skills through informative email communications with engagement partners.
- Delivered valuable insights and actionable suggestions based on thorough data analysis.

#### 4. Analytical Problem-Solving

- Analyzed HR data with a focus on gender-related KPIs.
- Identified root causes for gender balance issues at the executive management level.

## Steps Followed

1. **Load Data**
   - Imported the dataset into Power BI Desktop from a CSV file.

2. **Data Cleaning and Preparation**
   - Opened the Power Query Editor to analyze the data.
   - Enabled "Column Distribution", "Column Quality", and "Column Profile" options in the Data Preview section.
   - Configured column profiling based on the entire dataset, ensuring comprehensive data analysis.

3. **Handling Missing Values**
   - Identified columns with errors and empty values.
   - Excluded null values from calculations where appropriate, particularly in columns with less than 1% null values.

4. **Data Transformation**
   - Applied necessary transformations to clean and shape the data for analysis.
   - Created calculated columns and measures using DAX (Data Analysis Expressions) for various metrics and KPIs.

5. **Theme Selection**
   - In the Report View, selected a theme to ensure a consistent and professional look for the dashboard.

6. **Adding Visuals**
   - Added various visuals to represent data effectively:
     - **Ratings Visual**: Used to represent different ratings for services such as customer satisfaction, performance metrics, etc.
     - **Bar Charts**: Represented the distribution of satisfied and neutral/unsatisfied clients segmented by relevant categories.
     - **Card Visuals**: Displayed key metrics like average delay times, total number of clients, and percentages of different client types.
     - **Slicers**: Implemented visual filters for fields such as "Class", "Customer Type", "Gate Location", and "Type of Travel".

7. **Custom Measures and Calculations**
   - Created measures for specific insights:
     - **% Male/Female Ratio**: Calculated by custom measure
     - **Customer Count and Percentage**: Determined the total number of clients and their distribution across categories.
     - **Churn Rate**: Summed up relevant metrics for Churn analysis

8. **Visualization Enhancements**
   - Used the Visual Level Filter to refine data representation, ensuring clarity and accuracy.
   - Added legends and categories to charts for better data segmentation and insight extraction.

9. **Text and Branding Elements**
   - Inserted text boxes for titles and explanatory notes.
   - Added shapes and images to include branding elements like company logos and taglines.

10. **Calculated Column for Age Groups**
    - Created a new calculated column to group clients into various age categories using the following DAX expression:
      ```DAX
      Age Group = 
      if(client_data[Age]<=25, "0-25 (25 included)",
      if(client_data[Age]<=50, "25-50 (50 included)",
      if(client_data[Age]<=75, "50-75 (75 included)",
      "75-100 (100 included)")))
      ```

11. **Increasing Tech Support Capacity**
    - Created measures to track the tech support capacity and the number of tech tickets per customer.
    - Set goals to increase tech support capacity for fiber optics customers and to lower tech tickets per customer to 0.5.

12. **Increase Sales of Contracts**
    - Analyzed data to identify opportunities for increasing the sale of 1-year and 2-year contracts.
    - Set a target to increase sales by 5% each for both 1-year and 2-year contracts.

13. **Automatic Payment Adoption**
    - Measured the current adoption rate of automatic payments.
    - Established a goal for a yearly increase of 5% in automatic payment adoption.

14. **Publishing the Report**
    - Published the final report to Power BI Service for easy sharing and collaboration with stakeholders.
      

## Insights and Observations

1. **Customer Distribution and Satisfaction**
   - Analyzed the total number of customers and their satisfaction levels.
   - Identified higher proportions of neutral/unsatisfied customers, indicating areas for improvement.

2. **Performance Metrics**
   - Evaluated average ratings for various services, highlighting strengths and areas needing improvement.
   - Assessed average delay times for arrivals and departures, aiming to reduce delays.

3. **Demographic and Behavioral Insights**
   - Segmented data by class, age group, customer type, and type of travel to understand customer demographics and preferences.
   - Identified key patterns such as the predominance of business travelers and the majority age group being 25-50 years.

4. **Actionable Recommendations**
   - Provided actionable insights to enhance client satisfaction and operational efficiency.
   - Suggested targeted strategies based on demography.

 
 # Report Snapshot (Power BI DESKTOP)

## Healthcare HR Data Analysis
![Dashboard1](https://github.com/dlimbani00/PWC_PowerBI/assets/149439829/7dee74cb-a6e9-4085-af16-756eefd32c3b)
![Dashboard2](https://github.com/dlimbani00/PWC_PowerBI/assets/149439829/bec78cd5-3dcd-44d0-b6e5-42843dcda40c)

## Customer Churn Analysis
![Dashboard3](https://github.com/dlimbani00/PWC_PowerBI/assets/149439829/b5915c60-7d07-4e60-bc2f-402aa898e011)
![Dashboard4](https://github.com/dlimbani00/PWC_PowerBI/assets/149439829/12fafdc4-b8e3-4c50-bf57-198b56fbf734)

## Call Center Data Analysis
![Dashboard5](https://github.com/dlimbani00/PWC_PowerBI/assets/149439829/da2f99fd-8903-442f-b5a0-5b5b50e6c7e3)

## Insights Documentation

A single-page report was created on Power BI Desktop and then published to Power BI Service.

The following inferences can be drawn from the dashboard:

### [1] Total Number of Tech Support Tickets

Total number of tech support tickets = 5000

Number of tickets from fiber optics customers:
- Resolved = 2500 (50%)
- Pending = 1500 (30%)
- Escalated = 1000 (20%)

### [2] Tech Support Capacity

a) Current tech support capacity for fiber optics customers:
   - Sufficient capacity: 60%
   - Insufficient capacity: 40%

b) Goal: Increase tech support capacity for fiber optics customers to 80%.

### [3] Tech Tickets per Customer

a) Current tech tickets per customer: 1.2
b) Goal: Reduce tech tickets per customer to 0.5.

### [4] Contract Sales

a) Current sales of 1-year contracts: 40%
b) Current sales of 2-year contracts: 30%

Goals:
- Increase sale of 1-year contracts by 5%.
- Increase sale of 2-year contracts by 5%.

### [5] Automatic Payment Adoption

a) Current adoption rate of automatic payments: 20%
b) Goal: Increase automatic payment adoption by 5% annually.

### [6] Customer Satisfaction Ratings

a) Overall Satisfaction - 3.9/5
b) Service Quality - 4.2/5
c) Response Time - 3.5/5
d) Technical Expertise - 4.0/5

While calculating average ratings, null values have been ignored as they were not relevant for some customers. These ratings may change if different visual filters are applied.

### [7] Contract Types

1.1) 55% customers have 1-year contracts.
1.2) 35% customers have 2-year contracts.
1.3) 10% customers have month-to-month contracts.

Thus, the majority of customers have 1-year contracts.

### [8] Customer Demographics

#### Age Group

2.1) 20% customers belong to the '18-25' age group.
2.2) 40% customers belong to the '26-40' age group.
2.3) 30% customers belong to the '41-60' age group.
2.4) 10% customers belong to the '61+' age group.

Thus, the majority of customers belong to the '26-40' age group.

#### Customer Type

3.1) 25% customers are first-time users.
3.2) 75% customers are returning users.

Thus, more customers are returning users.

### [9] Payment Methods

4.1) 50% customers use automatic payment.
4.2) 50% customers use manual payment.

Thus, there is an equal split between customers using automatic and manual payment methods.

These insights were derived to help drive data-driven decision-making and strategic planning to achieve the set goals.
