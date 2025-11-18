analysis/expo_analysis.md

# Tech Expo Operations Analysis

## Overview

This project analyzes operations and attendance data for a fictional Tech Expo.  
The goal is to identify trends, operational bottlenecks, and actionable insights that can support planning for future events. All data is **synthetic**, created for the purpose of demonstrating skills in:

- Data Analytics  
- Operations Management  
- Queue Modeling  
- Forecasting  
- Dashboarding  
- Project Management Documentation


1. Load Data
```python
import pandas as pd

attendees = pd.read_csv("../data/attendee_forecast.csv")
booths = pd.read_csv("../data/booth_data.csv")
staffing = pd.read_csv("../data/staffing_costs.csv")

attendees.head(), booths.head(), staffing.head()
```

2. Explore Attendee Trends
```python
attendees["total_attendees"] = (
    attendees["early_registrations"] +
    attendees["walk_ins"]
)

attendees.describe()
```

3. Peak Hour Analysis
```python
peak_hours = attendees.groupby("hour")["total_attendees"].mean()
peak_hours
```

4. Staffing Cost & Utilization
```python
staffing["total_cost"] = staffing["staff_count"] * staffing["cost_per_staff"]
staffing
```

5. Booth Performance
```python
booths["interaction_rate"] = (
    booths["visitors"] / booths["staff_assigned"]
)
booths.sort_values(by="interaction_rate", ascending=False)

```

Queue & Wait-Time Modeling (Conceptual)
Queue wait time follows the M/M/s queuing model:
λ = arrival rate
μ = service rate
s = number of staff serving
Key assumptions:
First-Come First-Served
Constant service time
No early VIP or prioritization
Placeholder formula (to be updated with real numbers later):
```python
arrival_rate = attendees["total_attendees"].max()
service_rate = 10  # persons/hour per staff
staff = 5
utilization = arrival_rate / (staff * service_rate)
utilization
```

Staffing Cost & Utilization
```python
staffing["total_cost"] = (
    staffing["staff_count"] * staffing["cost_per_staff"]
)
staffing
```

6. Key Insights Summary

- Peak attendee hours
- Under/overstaffed time blocks
- Booths with best interaction rates
- Cost per attendee

7. Assumptions

- Forecasted attendance is based on synthetic historical patterns.
- Queue times assume FIFO (first in, first out) flow.
- All staff are available the full day.
- Booth service rate is constant within each hour.
- No unexpected disruptions (weather, system outage, etc.).

8. Limitations

- Synthetic data may not reflect real-world randomness.
- Walk-in visitors can spike unpredictably.
- Booth interaction quality not measured (only quantity).
- Staffing efficiency varies by experience level.
- Simulation does not yet include probabilistic arrival patterns.

9. Recommendations

- Add Monte Carlo simulation for realistic arrival variability.
- Add optimization model using PuLP or OR-Tools.
- Integrate real-time sensor data for booth counting.
- Improve forecasting using ARIMA, Prophet, or ML models.
- Conduct sensitivity analysis for staffing cost changes.

