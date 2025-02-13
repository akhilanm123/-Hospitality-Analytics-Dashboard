# Hospitality-Analytics-Dashboard Using PowerBI
#### Power BI | DAX | Power Query | Data Visualization

## Project Overview
This Power BI dashboard provides actionable insights into hotel performance, booking trends, and revenue optimization. The dataset is a synthetic representation of real-world hospitality data and has been designed to analyze:
-  Revenue & Occupancy trends across different cities
-  Platform-wise booking efficiency & Realization %
-  Luxury vs. Business hotel performance
-  Weekday vs. Weekend stay patterns
## Technical Approach
#### 1. Data Processing
- Cleaned and transformed data using Power Query.
- Created custom DAX measures for KPIs like RevPAR, ADR, and Realization %.
#### 2. Key DAX Measures Used:
- Revenue = SUM(fact_bookings[revenue_realized])
- RevPAR = DIVIDE([Revenue],[Total Capacity])
- ADR = DIVIDE( [Revenue], [Total Bookings], 0)
  Realization % = 1 - ([Cancellation %] + [No Show rate %])
#### 3.  Data Visualization:
- Interactive filters for City, Room Type, and Date Ranges.
- Trend Analysis, Category-wise Revenue, and Platform Performance visualizations.
