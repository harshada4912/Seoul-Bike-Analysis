## 🚴‍♂️ Bike Rental Analysis Dashboard
## 📌 About the Project

The Bike Rental Analysis Dashboard is an interactive Power BI report built on the Seoul Bike Dataset, designed to analyze daily and seasonal bike usage trends.
It provides insights into how weather conditions, temperature, humidity, and time patterns impact the number of rented bikes — helping optimize operational decisions and understand user behavior.

🎯 Objective

- Identify factors influencing bike rentals.
- Discover seasonal and hourly trends.
- Evaluate the impact of weather and functioning days on rental counts.
- Build KPI-based insights for business decisions.


## 📊 Key Visuals and Insights


| Visualization                                      | Description                                               | Fields Used                                                 |
| -------------------------------------------------- | --------------------------------------------------------- | ----------------------------------------------------------- |
|  Rentals by Month (Column Chart)**                | Shows total rentals by month.                             | Month Name, SUM(Rented Bike Count)                          |
|  Rentals by Season (Bar Chart)**                  | Displays total rentals per season.                        | Season, SUM(Rented Bike Count)                              |
|  Hourly Rentals (Line Chart)**                    | Shows rental trends across different hours.               | Hour, SUM(Rented Bike Count)                                |
|  Top 10 Busiest Hours (Bar Chart)**               | Identifies hours with highest rentals.                    | Hour, SUM(Rented Bike Count)                                |
|  Rental by Weather Impact (Donut Chart)**         | Compares rentals by weather condition or functioning day. | Weather Condition / Functioning Day, SUM(Rented Bike Count) |
|  Humidity & Temperature vs Rentals (Area Chart)** | Shows how weather variables affect rentals.               | Temperature(°C), Humidity(%), SUM(Rented Bike Count)        |
|  Season + Temperature (Table)**                   | Displays average rentals by season and temperature.       | Season, Temperature(°C), AVERAGE(Rented Bike Count)         |
|  Hour vs Day Name (Treemap)**                     | Shows which day-hour combination has most rentals.        | Day Name, Hour, SUM(Rented Bike Count)                      |
|  Season Ranking by Month (Ribbon Chart)**         | Visualizes seasonal performance change over months.       | Month Name, Season, SUM(Rented Bike Count)                  |

