
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

Event Name: Tokyo Tech Expo 2025

Theme: AI, Robotics & Emerging Technologies

Location: Tokyo Big Sight (East Hall)

Duration: 1 Day (10:00 – 18:00 (8 hours))

Expected Visitors: 3,000 attendees

Event Areas Modeled
1. Registration Counter (check-in, badge printing)
2. Keynote Hall (two keynote sessions)
3. 20 Exhibitor Booths (varied traffic patterns)
4. Food Court
5. Walkway / General Area Traffic

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


# 7. Tools & Skills Demonstrated
- Excel (advanced): forecasting, scenario modeling
- SQL: data cleaning & aggregation
- Python (optional): forecasting models
- PowerBI / Tableau: dashboards
- Project Management: documentation, assumptions, risk & recommendations
- Operations Management: queuing models, staffing optimization

# 8. Status

In Progress
- Dataset: generating
- Forecasting: pending
- Dashboard: pending
- Summary: pending

# 9. Future Enhancements
- Add optimization using Python’s PuLP
- Add arrival simulation using Monte Carlo
- Add booth-level heatmap dashboards
  
