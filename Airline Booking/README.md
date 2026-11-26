# ✈️ Airline Booking Dashboard (Excel)

An interactive multi-page business intelligence dashboard built in **Microsoft Excel** analyzing airline booking performance, passenger behavior, and market demand across **79.6K total passengers**. Designed with a custom navigation sidebar, KPI cards, Pivot Charts, and dynamic Slicers (`trip_type`, `sales_channel`, and `flight_day`).

---

## 📊 Dashboard Pages & Screenshots

### 1. Overview
Focuses on overall booking funnel performance, completion rates, sales channels, and booking trends by trip type and flight day.

![Overview Page](images/Overview.png)

* **KPIs:** Total Passengers (`79.6K`), Incomplete Bookings (`84%`), Completed Bookings (`16%`), Avg of Purchase Lead (`85`), Avg of Passengers (`2`)
* **Visuals:**
  * **Booking Complete Rate:** Pie chart showing `16%` completed (`Yes`) vs. `84%` incomplete (`No`)
  * **Booking by Sales Channel:** Donut chart comparing `Internet` (`92%`) vs. `Mobile` (`8%`)
  * **Booking Completed over Trip Type:** Column chart led by `RoundTrip` (`7.45K`), followed by `OneWay` (`20`) and `CircleTrip` (`5`)
  * **Booking Completed by Flight Day:** Line chart across days of the week (`Sun`–`Sat`), peaking mid-week on `Wed` (`1.25K`) and `Mon` (`1.20K`)

---

### 2. Customer Behavior
Explores traveler preferences and trip characteristics such as add-on baggage demand, stay duration, seat preference alignment, and top origin markets.

https://github.com/mahamedtharwat/Data-Analysis-Projects/blob/523246c3fe292c915aa12d2eca85ccb4eb634725/Airline%20Booking/Dashboard/Customer%20Behavior.png

* **KPIs:** Total Passengers (`79.6K`), Wants Extra Baggage (`33.4K`), Avg of Purchase Lead (`85`), Avg Length of Stay (`23`), Avg of Flight Duration (`7`)
* **Visuals:**
  * **Max Length of Stay over Trip Type:** Treemap comparing `RoundTrip` (`778`), `OneWay` (`272`), and `CircleTrip` (`225`)
  * **Booking Completed over Wants Preferred Seat:** Pie chart split between `65%` (`No`) and `35%` (`Yes`)
  * **Top 10 of Origin over Booking Completed:** Bar chart ranked by completed bookings, led by `Malaysia` (`2,468`), `Australia` (`900`), `China` (`694`), and `Indonesia` (`615`)

---

### 3. Market Analysis
Highlights geographic reach, high-volume routes, and flight hour patterns to support commercial and operational planning.

![Market Analysis Page](images/Market%20Analysis.jpg)

* **KPIs:** Total Passengers (`79.6K`), Avg of Purchase Lead (`85`), Avg Length of Stay (`23`), Avg of Flight Hour (`9`), Avg of Flight Duration (`7`)
* **Visuals:**
  * **Top 10 of Origin over Booking Completed:** Filled Map chart highlighting completed bookings across markets (`131` to `2,468`)
  * **Top 10 Route over Booking Completed:** Area chart tracking completed bookings across top city-pair/route codes
  * **Top 10 Flight Hours over Booking Completed:** Column chart showing completed bookings across flight hour buckets (peaking at `1,660`)

---

## 🎛️ Interactive Filters (Excel Slicers)
* **Trip Type (`trip_type`):** `CircleTrip`, `OneWay`, `RoundTrip`
* **Sales Channel (`sales_channel`):** `Internet`, `Mobile`
* **Flight Day (`flight_day`):** `Sun`, `Mon`, `Tue`, `Wed`, `Thu`, `Fri`, `Sat` *(available on Market Analysis)*

---

## 💡 Key Insights
* **High Abandonment / Incomplete Rate:** `84%` of bookings remain incomplete (`16%` completion rate), signaling a major opportunity to optimize checkout flows.
* **Web-Dominated Bookings:** `92%` of bookings occur via `Internet` compared to `8%` on `Mobile`.
* **Round-Trip Dominance:** `RoundTrip` accounts for the overwhelming majority of completed bookings (`7.45K`) and the longest maximum stay (`778`).
* **Top Geographic Markets:** `Malaysia` (`2,468`) leads completed bookings by a wide margin, followed by `Australia` (`900`) and `China` (`694`).

---

## 🛠️ Tools & Excel Features Used
* **Microsoft Excel** (`.xlsx`)
* **Pivot Tables & Pivot Charts:** Dynamic data aggregation and visualization (Pie, Donut, Bar/Column, Line, Area, Treemap, and Map charts)
* **Slicers & Report Connections:** Cross-sheet interactive filtering across KPI cards and charts
* **Formulas (`GETPIVOTDATA`, `AVERAGE`, `COUNT`, `MAX`):** Dynamic KPI card values linked to Pivot Tables
