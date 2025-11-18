
# Tokyo Tech Expo: Staffing & Operations Optimization

Data-driven modeling for a 3,000-attendee Tech Expo at Tokyo Big Sight

# 1. Overview

This project analyzes and optimizes operations for a one-day Tech Expo at Tokyo Big Sight.

It includes:

- Attendee Forecasting
- Queue + Wait Time Estimation
- Staffing Optimization
- Cost Scenarios
- PM-Style Documentation
- Dashboards + Insights
  
This project showcases skills across project management, data analytics, and operations.

# 2. Objectives

- Predict visitor attendance throughout the day
- Estimate queue times at registration and booths
- Determine optimal staffing levels
- Analyze cost scenarios under different service levels
- Visualize insights through a dashboard
- Document findings using PM-style structure

# 3. Event Scenario

- Event Type: AI & Technology Expo (customizable)
- Location: Tokyo Big Sight
- Expected Attendance: 3,000 visitors
- Duration: 10 AM – 6 PM (8 hours)
- Areas Modeled:
  - Registration
  - Keynote Stage
  - 20 Exhibitor Booths
  - Food & Beverage
 

# 4. Dataset Description

This repository contains synthetic, realistic datasets:
| File                    | Description                         |
| ----------------------- | ----------------------------------- |
| `attendee_forecast.csv` | Expected arrivals per hour          |
| `staffing_costs.csv`    | Cost per staff type                 |
| `booth_data.csv`        | Booth-level traffic + service rates |


# 5. Methodology
1. Forecasting

Used simple time-series or distribution assumptions to model hourly arrivals.

2. Queue Simulation

Calculated expected wait times using:
- Arrival rate
- Service rate
- Number of staff

5. Staffing Optimization

Modeled scenarios:
- Minimal staffing
- Balanced service
- Premium service
- Cost vs service-level trade-off

6. Dashboard

Created a visual dashboard summarizing results:
- Visitor flow
- Costs
- Wait time predictions
- Recommendations

7. PM Documentation

Included:
- Scope definition
- Assumptions
- Constraints
- Risks
- Recommendations
  
# 6. Key Outputs
- Staffing Model (Excel)
- Forecast & Traffic Model
- Cost Scenarios
- Dashboard (.png / .pbix)
- PM Case-Study Summary


# 7. Repository Structure

├── data/
│   ├── attendee_forecast.csv
│   ├── staffing_costs.csv
│   └── booth_data.csv
│
├── analysis/
│   ├── staffing_model.xlsx
│   ├── forecast.ipynb
│   └── sql_queries.sql
│
├── dashboard/
│   ├── expo_dashboard.png
│   └── expo_dashboard.pbix
│
├── README.md
└── LICENSE

# 8. Tools & Skills Demonstrated
- Excel (advanced): forecasting, scenario modeling
- SQL: data cleaning & aggregation
- Python (optional): forecasting models
- PowerBI / Tableau: dashboards
- Project Management: documentation, assumptions, risk & recommendations
- Operations Management: queuing models, staffing optimization

# 9. Status

In Progress
- Dataset: generating
- Forecasting: pending
- Dashboard: pending
- Summary: pending

# 10. Future Enhancements
- Add optimization using Python’s PuLP
- Add arrival simulation using Monte Carlo
- Add booth-level heatmap dashboards
  
