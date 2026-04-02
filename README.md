# Accident-Report-Dashboard

## Preview of the Dashboard

#### Overview Dashboard
![](image/OverviewDashboard.png)

## Key Insights:
1. Safety Performance Trends - Between 2022 and 2024, total accidents declined slightly by 0.9% (from 6,117 to 6,061), yet the Risk Score increased from 0.43 to 0.44, suggesting a rise in the severity or impact per incident. Despite the marginal reduction in frequency, casualty figures remained persistently high, indicating limited progress in reducing overall harm. However, in the first four months of 2025, recorded accidents fell to 1,734, representing a decrease of 230 compared to the same period last year, accompanied by a significant reduction of 318 total casualties
   
3. Accident Severity & Visibility - The distribution of accident types has remained remarkably consistent, indicating that underlying environmental and behavioral factors continue to persist. Minor accidents account for the largest share, comprising approximately 47–48% of all incidents, followed by major and fatal accidents, each contributing around 25–26%. In terms of visibility, nearly half of all accidents, approximately 49–50%, occur under high visibility conditions, suggesting that driver behavior, such as overspeeding or distraction, plays a more significant role than adverse environmental conditions. Meanwhile, medium and low visibility conditions collectively account for the remaining 50% of incidents.
   
5. Temporal and Geographic Insights - Each year demonstrates a distinct linear accumulation of accidents and casualties. Data reveals a consistent upward trend beginning in July and peaking in December. While Chandigarh recorded the highest accident volume in 2022 with 809 incidents, Mumbai and Chennai emerged as the highest-volume cities by 2024, each reporting 775 accidents. 

## Procedure for creating a dashboard from raw dataset to data visualization

### Data Cleaning
In these phase I used Excel to:
1. Standardizing Data
   - Fix the inconsistent formats
   - Standardize units, naming conventions, and categories
2. Handling Missing Values
   - Identify null or blank entries. I use fill down function to fill the blank records
3. Removing Duplicates
   -Detect duplicate rows in accident_ID column and remove it.
4. Correcting Data Types
   - Convert columns to appropriate formats (e.g., date, numeric, text)

### Data Modeling and Measure Development
In this phase, Power BI was utilized to design the data model and develop appropriate measures to support analysis and reporting.
1. A calendar table is created based on the minimum and maximum date values to ensure a continuous and complete time dimension.
2.A dedicated calculation table was established to centralize and organize key measures, improving the overall structure and maintainability of the data model.
3. DAX was utilized to develop measures that enable dynamic visualizations, allowing reports to automatically reflect changes in key metrics such as accident frequency, casualty counts, and growth trends.
4. Measures and KPI's
   - Year-to-date (YTD) measures were computed for total accidents and casualties, as well as the average risk score, to present a consolidated view of performance within the current reporting period.
   - Previous-Year-to-date (PYTD) measures were computed for total accidents and casualties, as well as the average risk score, to present a consolidated view of performance within the current reporting period.
   - Difference of YTD and PYTD  in terms of accidents, casualties, and risk scores.
   - Year-over-year (YoY) percentage growth or changes were analyzed for accidents, casualties, and risk scores to assess performance relative to the same period in the prior year.

### Data Visualization and Chart Requirements
1. Cards that shows summary of the year-to-date (YTD) performance compared to the previous year.
   - YTD Accidents
   - YTD Casualties
   - YTD Risk Score
2. Map Visualization that displays the geographical distribution of accidents.
3. A Pie Chart that breaks down the severity of the people involved in accidents such as minor, major and fatal.
4. A pie chart illustrating the distribution of accidents by environmental visibility, categorized into low, medium, and high visibility levels.
5. Topographic Information (Table) that provides a granular, city-level comparison of safety metrics.
6. A Bar chart that shows the cause and total accidents.
7. Trends by Month that shows the total accident, casualties and number of vehicles involved per accidents

## Disclaimer
The insights and dashboard presented in this report are for educational and demonstration purposes only.
Data Source: The analysis is based on a publicly available dataset from Kaggle.
Contextual Accuracy: This project was developed to showcase proficiency in data cleaning (Excel), data modeling (Power BI, DAX), and technical storytelling. 
Non-Official Status: This report is not affiliated with any government transport authority or road safety organization. For official safety statistics or policy guidance, please refer to the relevant national or local transportation departments.

## Reference 
The dataset was downloaded from kaggle 
[Indian Road Accident Dataset (2022–2025)]([https://youtu.be/uPkemycepLc?si=NhYM72UR_J_zB6EZ](https://www.kaggle.com/datasets/sehaj1104/indian-road-accident-dataset-20222025))
