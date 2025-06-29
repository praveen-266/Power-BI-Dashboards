## **RedBus Booking Insights Dashboard — A Power BI-Powered Travel Analytics Solution**

---

## 🧩 Problem Statement

RedBus, India’s largest intercity bus booking platform, handles millions of user interactions, but lacks contextual visibility into **regional travel behavior**, **seasonal spikes**, and **festival-driven surges** across its route network. This makes it difficult for stakeholders to **forecast demand**, **optimize routes**, and **plan campaigns** effectively.

---

## 🧠 Project Overview

This project aims to build a **real-world, end-to-end Business Intelligence solution** that:
* Aggregates booking and search data from RedBus
* Enriches it with **live Indian festival dates (Calendarific API)**
* Applies **feature engineering** for behavior segmentation
* Delivers a **professional Power BI dashboard** to visualize trends, seasonality, and cultural impact on route performance

---

## 🎯 Why I Selected This Project (Business Problem Solved)

RedBus operates in a demand-sensitive market highly influenced by festivals, weekends, and school holidays. Yet, traditional dashboards fail to account for such **external behavioral triggers**.
With this solution, I aimed to:

* **Simulate a real-world stakeholder dashboard** use case
* Show how **cultural context + data = better decisions**
* Present **actionable insights** like identifying most profitable routes or peak demand seasons
* Highlight the value of **API enrichment** in decision-making

---

## 📊 Project Results & Business Insights

### 📌 Top Insights Identified:

1. **Regional Leader**: South Indian routes dominated bookings — **Tamil Nadu ranked #1** consistently across all time frames.
2. **Monthly Trends**:

   * **December** had the highest bookings (holiday & vacation period)
   * Followed by **May**, due to summer breaks
   * **February** saw the **lowest activity**
3. **Weekday Behavior**:

   * **Sunday** ranked highest for seat bookings
   * **Tuesday** was consistently the lowest
4. **Seasonal Patterns**:

   * **Monsoon** topped seat bookings (possibly linked to festivals and return travel)
   * **Autumn** showed the least activity
5. **Tier-wise Dynamics**:

   * For Tier-1 origin routes (T1 → T1, T1 → T2, T1 → T3): **Friday** and **Sunday** peaked
   * For Tier-2/3/4 origins: **Sunday** and **Monday** dominated

---

## 📦 Tools & Tech Stack Used

| Tool                   | Purpose                                                      |
| ---------------------- | ------------------------------------------------------------ |
| **Python + Pandas**    | Data wrangling, feature engineering, Holiday API integration |
| **Calendarific API**   | Injected real Indian festival dates (2023–2025)              |
| **Power BI**           | Full-stack dashboard: filters, visuals, DAX columns          |
| **Custom DAX Columns** | Festival Indicators, Top Ranked Routes                       |

---

## 📊 Power BI Dashboard Features

* **Filters/Slicers**:

  * Date of Journey
  * Source & Destination Region
  * Source & Destination Tier

* **Metrics Visualized**:

  * `total_seats_booked`
  * `total_search_count`
  * `is_festival` (Festival indicator column)

* **Key Visuals**:

  * Bookings by **Weekday**, **Month**, **Season**
  * **Tier vs Tier** route performance
  * **Festival impact** across geographies

---

## 🧩 DAX Logic Highlights

* `Festival_Indicator`: Flag festival vs non-festival travel demand
* `Top_Ranked_Route`: Dynamic ranking of best-performing routes

These DAX columns were key in enabling users to **filter behavior based on time or festival**, answering questions like:

* *“Which routes surge during major Indian festivals?”*
* *“How do Tier-3 cities behave around national holidays?”*

---

## ✅ Project Conclusion

This project simulates a **production-grade BI solution** — from ingestion to enrichment to dynamic visualization. It reflects how **cultural data fusion**, like integrating a festival API, can drive **richer business intelligence**, enabling:

* Better route planning
* Campaign timing optimization
* Regional marketing insights
* Operational cost savings through demand prediction

---

## 🌍 Business Impact & Real-World Application

This methodology can empower companies like RedBus, MakeMyTrip, or even IRCTC to:

* **Pre-emptively scale fleet or promotions around festivals**
* **Reallocate marketing budgets** to high-conversion regions and routes
* **Design tier-based loyalty programs** based on travel behaviors
* **Predict demand dips or surges** to optimize pricing

---

## 💬 Final Thoughts (LinkedIn CTA Style)

If you’re a hiring manager looking for a **BI-ready data analyst**, let’s connect! This project showcases my ability to:

* Build **full-stack dashboards** with real-world logic
* Integrate **external APIs** for business enrichment
* Use **Python + Power BI + DAX** in an analyst pipeline
* Present **data as decisions**, not just visuals

Let’s build insights that *move businesses forward.*
