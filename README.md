# Hospitality-Analytics-Dashboard Using PowerBI
#### Power BI | DAX | Power Query | Data Visualization

## Project Overview
This Power BI dashboard provides actionable insights into hotel performance, booking trends, and revenue optimization. The dataset is a synthetic representation of real-world hospitality data and has been designed to analyze:
-  Revenue & Occupancy trends across different cities
-  Platform-wise booking efficiency & Realization %
-  Luxury vs. Business hotel performance
-  Weekday vs. Weekend stay patterns
## Dataset Used
- <a href="https://github.com/akhilanm123/-Hospitality-Analytics-Dashboard/blob/main/dim_date.csv">Dates</a>
- <a href="https://github.com/akhilanm123/-Hospitality-Analytics-Dashboard/blob/main/dim_hotels.csv">Hotels</a>
- <a href="https://github.com/akhilanm123/-Hospitality-Analytics-Dashboard/blob/main/dim_rooms.csv">Rooms</a>
- <a href="https://github.com/akhilanm123/-Hospitality-Analytics-Dashboard/blob/main/fact_aggregated_bookings.csv">fact_aggregate_bookings</a>
- <a href="https://github.com/akhilanm123/-Hospitality-Analytics-Dashboard/blob/main/fact_bookings.csv">fact_bookings</a>
## Technical Approach
#### 1. Data Processing
- Cleaned and transformed data using Power Query.
- Created custom DAX measures for KPIs like RevPAR, ADR, and Realization %.
#### 2. Key DAX Measures Used:
- Revenue = SUM(fact_bookings[revenue_realized])
- RevPAR = DIVIDE([Revenue],[Total Capacity])
- ADR = DIVIDE( [Revenue], [Total Bookings], 0)
- Realization % = 1 - ([Cancellation %] + [No Show rate %])
###### A total of 23  DAX formulas were used in this project. For a full list of all formulas, check the Complete DAX Formulas Document - <a href="https://github.com/akhilanm123/-Hospitality-Analytics-Dashboard/blob/main/DAX%20Formulas.xlsx">DAX Formulas</a>
#### 3.  Data Visualization:
- Interactive filters for City, Room Type, and Date Ranges.
- Trend Analysis, Category-wise Revenue, and Platform Performance visualizations.
## Dashboard Interaction
-<a href="https://github.com/akhilanm123/Hospitality-Analytics-Dashboard/blob/main/HD.pbix">Hospitality-Analytics-Dashboard</a>
## Dashboard
![image](https://github.com/user-attachments/assets/f679d8ea-4029-468e-8760-08d9a8321aae)


## Key Performance Indicators (KPIs) Tracked
- Revenue – Total revenue generated across properties.
- RevPAR (Revenue per Available Room) – Measures revenue efficiency.
- ADR (Average Daily Rate) – Average revenue per booking.
- Occupancy % – Measures room utilization.
- Realization % – Identifies booking completion rate after cancellations & no-shows.
- Platform-wise Performance – Analyzes efficiency of different booking sources.
-  City-Wise Performance – Compares hotel performance across different locations
  ## Key Insights & Business Impact
 #### 1. Booking Platform Performance & Realization %
- Direct Offline Bookings had the highest Realization % (~70.09%), meaning fewer cancellations and no-shows.
- Tripster had a lower realization rate (~69.80%), indicating a higher rate of cancellations or no-shows.
- MakeYourTrip and Direct Online platforms showed slightly lower efficiency compared to offline bookings.
- Cancellations and no-show rates significantly impact revenue, with some platforms experiencing up to 25% cancellation rates.
 #### 2. Revenue & Occupancy Analysis by City
- Bangalore contributed the highest revenue (~81M), followed by Mumbai and Delhi.
- Occupancy % was highest in Bangalore (65.53%), while Delhi (53.40%) and Mumbai (53.07%) had lower occupancy.
- Cities with lower occupancy may have pricing or demand issues, leading to revenue loss.
- Revenue per available room (RevPAR) showed significant variation across cities, indicating pricing inconsistencies.
#### 3. Luxury vs. Business Hotels - Revenue Contribution & Performance
- Business hotels contributed 61.62% of total revenue, while luxury hotels contributed 38.38%.
- Luxury hotels had higher ADR (Average Daily Rate) but lower occupancy, meaning fewer bookings at higher prices.
- Business hotels had consistently higher occupancy, likely due to corporate travel demand.
 #### 4. Weekday vs. Weekend Performance
- Weekend occupancy (62.64%) was significantly higher than weekday occupancy (55.85%).
- Despite similar ADR on weekdays and weekends, RevPAR was higher on weekends due to better occupancy.
- Weekday revenue is lower due to fewer bookings, despite having more available rooms.
 #### 5.  Cancellation & No-Show Rate Impact on Revenue
- The average cancellation rate was 24.84%, leading to significant revenue loss.
- No-show rates were particularly high on online platforms, reducing overall realization %.
- Some booking platforms had 30%+ cancellation rates, severely affecting projected revenue.
 ### Tooltip Usage in KPI Visualizations
 Tooltips provide additional insights into key performance indicators (KPIs) by displaying specific data points when hovered over. This enhances data interpretation and enables better business strategy and performance evaluation. There are 6 tooltips used in the dashboard, all the details has be documented. Please click the file to know more about it -<a href="https://github.com/akhilanm123/-Hospitality-Analytics-Dashboard/blob/main/Tooltip%20Usage%20in%20KPI%20Visualizations.pdf">Tooltip </a>

## Final Conclusion 
This project delivers a comprehensive KPI analysis framework to track and optimize key business metrics. By leveraging data visualization and revenue tracking, it provides actionable insights for strategic decision-making.
#### Key Outcomes:
- Revenue & Market Segmentation: Tracks weekly revenue for Business & Luxury segments, aiding pricing and forecasting.
- Occupancy & Performance: Identifies weekday vs. weekend trends for better resource planning.
- Pricing Optimization: ADR and RevPAR insights support competitive pricing strategies.
- Enhanced Data Interpretation: Interactive tooltips improve clarity and usability.
-  Strategic Business Intelligence: Enables real-time KPI tracking for data-driven decisions.

This project transforms raw data into business intelligence, offering a scalable, data-driven approach for revenue management and operational efficiency.
