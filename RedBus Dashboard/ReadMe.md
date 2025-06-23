## 🚍 **Power BI Project: RedBus Booking Insights Dashboard (Festival-Aware + Tier-Wise)**


![RedBus Dashboard](https://github.com/user-attachments/assets/292a1b47-27bb-4fa9-9fa3-8f180e77f244)

🔴 **About RedBus:**
RedBus is India’s largest online bus ticketing platform, connecting millions of users across cities, regions, and states. With massive intercity booking data and seasonal peaks, RedBus presents an ideal opportunity to build a real-world, analytics-driven dashboard.

---

### 🎯 What I Built:

A **full-stack Power BI Dashboard** that tracks:

* Regional booking trends
* Tier-wise route performance
* Cultural & festival-based travel spikes
* Daily and monthly behavioral patterns

I also **integrated live Indian festival data using a Holiday API**, enriched it with multiple engineered features in Python, and visualized it with dynamic interactivity in Power BI.

---

### 🧰 Tools & Tech Stack:

* **Python + Pandas**: Data cleaning, feature engineering, API integration
* **Calendarific API**: Indian festival holidays (2023–2025) injected into dataset
* **Power BI**: Full interactive dashboard creation + professional branding

---

### 🔧 Power BI Implementation:

✅ **Filters / Slicers Used:**

* `doj` *(Date of Journey)*
* `srcid_region`
* `destid_region`
* `srcid_tier`
* `destid_tier`

✅ **Key Metrics Visualized:**

* 🎯 `total_seats_booked`
* 🔍 `total_search_count`
* 🎉 `is_festival` → to analyze booking spikes around Indian festivals

✅ **Behavioral Charts:**

* Average seats booked by:

  * **Weekday**
  * **Month**
  * **Season**
* Tier vs Tier route performance
* Festival impact across regions

---

### 📐 Custom DAX Columns:

```dax
-- Top Ranked Route Based on Seats Booked
Top_Seats_Rank = 
RANKX(
    ALLSELECTED('RedBus_final_data'[srcid_region], 'RedBus_final_data'[destid_region]),
    CALCULATE(SUM('RedBus_final_data'[total_seats_booked])),
    ,
    DESC,
    DENSE
)

-- Festival Indicator
is_festival = IF(NOT(ISBLANK([festival_name])), TRUE(), FALSE())
```

These columns were pivotal in allowing users to:

* See how festivals influenced seat bookings
* Spot which inter-regional routes consistently performed best

---

### 🌐 See it in Action:

📎 **Power BI Dashboard (Public Link)**
🔗 https://app.powerbi.com/your-dashboard-link](https://app.powerbi.com/groups/me/reports/5239e14c-2292-45c0-a02e-79be2d9fc8d3/8fd1773bc1806cb6a619?experience=power-bi


### 💼 Why This Project Matters:

✅ Simulates a real analytics use case
✅ Integrates API data (Calendarific) to add business context
✅ Covers the **entire pipeline** — from raw data → API integration → feature engineering → visualization
✅ Shows capability to handle **stakeholder-focused BI tools**
✅ Designed with **professional theming & brand-aligned visuals**

---

📢 **To Recruiters & BI Leaders**:
If you're hiring for a Data Analyst or BI role, I’d love to connect! This dashboard reflects my readiness to build and own analytics solutions that power decision-making.

🔎 Let’s connect and explore opportunities!
