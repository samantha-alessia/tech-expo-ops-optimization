analysis/expo_analysis.md

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
booths["interaction_rate"] = booths["visitors"] / booths["staff_assigned"]
booths
```

6. Key Insights Summary (Markdown)

- Peak attendee hours
- Under/overstaffed time blocks
- Booths with best interaction rates
- Cost per attendee
