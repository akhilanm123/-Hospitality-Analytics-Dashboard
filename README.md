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
###### A total of 23  DAX formulas were used in this project. For a full list of all formulas, check the Complete DAX Formulas Document 
#### 3.  Data Visualization:
- Interactive filters for City, Room Type, and Date Ranges.
- Trend Analysis, Category-wise Revenue, and Platform Performance visualizations.
