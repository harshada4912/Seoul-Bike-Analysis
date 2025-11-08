

## 🚴‍♂️ Bike Rental Analysis Dashboard
## 📌 About the Project

The Bike Rental Analysis Dashboard is an interactive Power BI report built on the Seoul Bike Dataset, designed to analyze daily and seasonal bike usage trends.
It provides insights into how weather conditions, temperature, humidity, and time patterns impact the number of rented bikes — helping optimize operational decisions and understand user behavior.

🎯 Objective

- Identify factors influencing bike rentals.
- Discover seasonal and hourly trends.
- Evaluate the impact of weather and functioning days on rental counts.
- Build KPI-based insights for business decisions.

## 🧩 Dataset Description  

| Column Name | Description |
|--------------|-------------|
| Date | Date when rentals were recorded |
| Bike_Count | Number of bikes rented during that hour |
| Hour | Hour of the day (0–23) |
| Temperature_C | Air temperature (°C) |
| Humidity | Relative humidity (%) |
| DewPoint_C | Dew point temperature (°C) |
| Rainfall_mm | Rainfall in millimeters |
| Season | Season of the year (Winter, Spring, Summer, Autumn) |





## 🧹 Data Cleaning Summary (Power Query Steps)  

| Step | Description |
|------|-------------|
| 1 | Imported CSV dataset into Power BI |
| 2 | Removed duplicates, blanks, and error rows |
| 3 | Added calculated columns: Day_Name, Month_Name, Year, Weekday_Weekend |
| 4 | Fixed data types for all fields |



## 💡 Key KPIs (Performance Indicators)  


| **KPI**                                | **Description**                                       | **Formula / DAX Expression**                                                              |
| -------------------------------------- | ----------------------------------------------------- | ----------------------------------------------------------------------------------------- |
| **Total Precipitation (mm)**           | Total rainfall accumulated over the recorded period   | `SUM(Rainfall_mm)`                                                                        |
| **Total Bikes**                        | Total number of bikes rented                          | `SUM(Rented_Bike_Count)`                                                                  |
| **Average Bikes/Day**                  | Average number of bikes rented per day                | `AVERAGE(Rented_Bike_Count)`                                                              |
| **Average Wind Speed (m/s)**           | Mean wind speed recorded during rentals               | `AVERAGE(Wind_speed(m/s))`                                                                |
| **Total Rentals in Peak Hour**         | Number of rentals during the hour with highest demand | `MAXX(SUMMARIZE(SeoulBike, [Hour], "Total", SUM(SeoulBike[Rented_Bike_Count])), [Total])` |



## 🧭 Filters and Slicers Used  

| Filter | Description |
|---------|-------------|
| Season | Filter data by season |
| Month | Filter by Month_Name |
| Functioning Day | Filter by operational status |

These slicers make the dashboard fully **interactive** and **user-friendly** for deeper insights.



## 📊 Dashboard Visuals  

### **Page 1: Overview Dashboard**
- 📈 Line Chart – Daily Rentals Over Time  
- 🌤️ Column Chart – Rentals by Month
- 📅 Bar Chart – Sum of Bikes by Functioning Day 
- ☀️ Scatter Plot – Total Bikes by Temperature (°C) 
- 💧Donut Chart –Count of Month by Seasons
- 🕓 Combo Chart – Rentals & Temperature by Month – Combo Chart

---
### **Page 2: Analysis**
- 💧 Pie chart-Count of Month by Seasons
- 📈 Line chart-Average of Rented Bike Count by Hour
- 📅 Bar chart-Average of Rented Bike Count by Day
- 📅 Stacked bar chart-Top 10 Busiest Hours by Rentals

  
---

## 🧠 Insights & Findings  

The Seoul Bike Analysis reveals several interesting patterns and operational insights. The data shows that summer and autumn record the highest bike rentals, while winter has the lowest, mainly due to cold weather and reduced outdoor activity. Peak rental hours occur between 8–9 AM and 5–7 PM, aligning perfectly with office commute times, indicating that the bike-sharing system is heavily used for daily transportation.Temperature plays a significant role in influencing rentals the ideal temperature range of 20–28°C results in maximum usage, as most riders prefer comfortable weather conditions. In contrast, rainy days significantly reduce rentals, showing that adverse weather discourages riders. Similarly, high humidity levels negatively correlate with the rental count, as users tend to avoid uncomfortable riding conditions.


## 🛠️ Tools and Technologies Used  

- **Power BI Desktop** – Data cleaning, transformation & visualization  
- **Microsoft Excel** – Initial review & structure checking  
- **Power Query Editor** – Data wrangling & custom column creation  
- **CSV Dataset** – Source file format  



## 📷 Dashboard
**Figure 1:**  Overview 
<img width="1312" height="741" alt="Screenshot 2025-11-08 150908" src="https://github.com/user-attachments/assets/1f0f40af-4906-4799-983d-70a45cf98dec" />

- **Figure 2:** Detailed
<img width="1305" height="727" alt="Screenshot 2025-11-08 150924" src="https://github.com/user-attachments/assets/e34b3397-cb14-4eb2-a0cd-fc482d5cbcc1" />

---

## 📎 Author  

**👤 Name:** Harshada pawar
**📧 Email:** [harshadapawar4912@gmail.com](mailto:prafullwahatule@gmail.com)  
**💻 GitHub:** [harshada4912](https://github.com/harshada4912)  
