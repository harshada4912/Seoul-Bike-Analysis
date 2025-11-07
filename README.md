

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
