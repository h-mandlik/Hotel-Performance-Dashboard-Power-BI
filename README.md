## 🏨 Hotel Performance Dashboard – Power BI  

This project analyzes **hotel performance metrics** such as **Revenue**, **Occupancy Rate**, **ADR (Average Daily Rate)**, and **Realization %** through an **interactive Power BI dashboard**.  

The dashboard provides **actionable insights** for stakeholders by visualizing property performance, booking trends, and platform analysis.  

---

## 📊 Dashboard Overview  

![Hotel Dashboard](666da50d-8d0c-4e87-ad10-e07ac7b6e5a6.png)  

**Key Dashboard Sections:**  
- **KPI Cards:** Revenue, Occupancy %, ADR, DSRN, Realization % (with WoW change)  
- **Revenue by Category:** Luxury vs Business  
- **Trend by Key Metrics:** RevPAR, ADR, Occupancy % over weeks  
- **Property-Wise Metrics:** Revenue, Bookings, ADR, RevPAR, Occupancy %, Realization %  
- **Platform Analysis:** Realization % vs ADR comparison  
- **Dynamic Filters:** City and Room Class  

---

## 🗂️ Dataset  

This dashboard was built using a **Hotel Booking Dataset** with the following fields:  
- Property Details: `property_id`, `property_name`, `city`, `room_class`  
- Booking Metrics: `total_bookings`, `DBRN`, `DSRN`, `DURN`  
- Revenue Metrics: `Revenue`, `ADR`, `RevPAR`  
- Performance Metrics: `Occupancy %`, `Realization %`, `Cancellation %`, `Average Rating`  

---

## 🛠️ Tools & Techniques  

- **Power BI** – Dashboard creation & interactivity  
- **Power Query** – Data cleaning & transformation  
- **DAX Measures** for key metrics:  
  
  -- Revenue per Available Room (RevPAR)
  RevPAR = DIVIDE([Revenue], [AvailableRoomNights])

  -- Realization Percentage
  Realization% = DIVIDE([UtilizedRoomNights], [BookedRoomNights]) * 100

  -- Average Daily Rate (ADR)
  ADR = DIVIDE([Revenue], [BookedRoomNights])
  

---

## 🚀 Key Insights
1. Top Performing Properties: Atiq Exotica (Mumbai) and Atiq Palace (Mumbai) are revenue leaders.

2. Weekend Occupancy exceeds weekday occupancy (62.6% vs 55.8%).

3. Luxury Category contributes 61.62% of revenue.

4. Direct Offline Platform yields the highest Realization % (~70.3%).

5. Portfolio Snapshot:

• Revenue: 1.69B

• Occupancy: 57.8%

• ADR: 12.70K

• Realization: 70.1%
