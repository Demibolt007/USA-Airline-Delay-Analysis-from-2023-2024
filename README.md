# USA Airline Delay Analysis (2023–2024)

This project analyzes real-world U.S. airline arrival and delay data from 2023 to 2024 to uncover operational trends, delay drivers, and performance patterns across airlines and airports. The goal is to provide actionable insights that can help improve on-time performance, operational planning, and customer experience.

This analysis was developed as part of the **FP20 Analytics Challenge 23** in collaboration with **ZoomCharts**, focusing on building interactive, business-ready Power BI dashboards with advanced drill-down capabilities.

---

## Project Objectives

Airline delays create significant inconvenience for passengers while increasing operational and financial pressure on airlines and airports. This project aims to understand when and where delays occur most frequently, what factors contribute most to delays, and which airlines and airports consistently perform better or worse. By identifying seasonal trends, carrier performance differences, and major delay drivers, this analysis supports data-driven decision-making for improving scheduling, resource allocation, and contingency planning.

---

## Dataset

U.S.A Airline Delay Analysis from 2023 - 2024(is included in this repository and can be downloaded directly.)

### Key Fields in the Dataset

| Category | Columns |
|--------|--------|
| Time | Year, Month |
| Airline | Carrier ID, Carrier Name |
| Airport | Airport Code, Airport Name, Latitude, Longitude |
| Flight Volume | Total Flights Arrival |
| Delay Count | Arrivals >15 Min Delay |
| Delay Causes (Count) | Carrier, Weather, National Aviation System, Security, Late Aircraft |
| Delay Duration (Minutes) | Minutes by each delay cause |
| Disruptions | Cancelled Flights, Diverted Flights |

---

## Key Business Questions Answered

1. What are the busiest months and airports for flights?
2. Which months experience the highest delay rates?
3. How do delay patterns vary across different airlines?
4. What are the primary causes of delays?
5. Which airports are most affected by weather-related delays?
6. How do delays differ between peak and off-peak seasons?
7. Are there geographic patterns in delay occurrences?
8. Do certain regions experience higher weather-related delays?
9. What percentage of flights are delayed over 15 minutes?
10. Which airlines and airports show the best on-time performance?

---

## Dashboard Structure (Power BI)

The report is designed using a in 2 pages and built on a **16:9 (1920×1080) canvas**.

### 📄 Page 1 — Flight Trends Overview

Focus: Overall traffic volume and operational disruptions.

**Visuals:**
- Total Flights vs Delays by Month
- Busiest Airports by Monthly Flight Volume
- Cancelled vs Diverted Flights by Month
- Percentage of Delayed Flights by Month
- Cancelled vs Diverted Flights Distribution (Pie Chart)

**KPI Cards:**
- Total Flights
- Delay Rate (%)
- Total Cancelled Flights
- Total Diverted Flights  
Each KPI includes year-over-year trend indicators using DAX.

---

### 📄 Page 2 — Delay Impact Analysis

Focus: Airline-level and geographic delay patterns.

**Visuals:**
- Delay Impact Distribution by Airline (Matrix)
  - Carrier Delay %
  - Weather Delay %
  - System Delay %
  - Late Aircraft Delay %
  - Security Delay %
- Flight Volume by Location (Map using Latitude & Longitude)
- Flight Volume by Carrier Name

---

<img width="2057" height="2368" alt="USA Airline Delay Analysis (2023–2024)" src="https://github.com/user-attachments/assets/9cc2b783-920f-47ee-813e-b55649188953" />

---

## Key Findings Summary

- November and January recorded the highest overall delay volumes.
- Atlanta (ATL), Dallas-Fort Worth (DFW), and Chicago O’Hare (ORD) are consistently the busiest airports.
- Late aircraft and carrier-related issues contribute more to delays than weather in most months.
- Certain airlines maintain lower delay ratios despite high flight volumes, indicating stronger operational efficiency.
- Weather-related delays are more concentrated in specific airport clusters, suggesting regional climate impact.

---

## Recommendations

- **We need to improve aircraft turnaround coordination** to reduce cascading late-aircraft delays.
- **I recommend increasing preventive maintenance scheduling** for airlines with high carrier-related delays.
- **We should improve weather contingency planning** at airports frequently affected by weather disruptions.
- **Airlines should adjust peak-season staffing models** to better handle volume surges.
- **Airports with persistent system delays need infrastructure and ATC coordination reviews.**

---

## Tools & Techniques Used

- **Power BI**
- **ZoomCharts Drill Down Visuals**
- DAX for:
  - Delay rates
  - Year-over-Year comparisons
  - KPI trend indicators
- Data modelling and calculated date fields
- Conditional formatting and interactive drill-downs

---

## How to Use This Repository

1. Download or clone the repository:
   ```bash
   git clone https://github.com/Demibolt007/USA-Airline-Delay-Analysis-from-2023-2024.git
