# Uber-Fare-Project: NYC Ride Insights with Python & Power BI

**A Deep-Dive Analytical Report on Uber Rides in NYC**

**Student:** Uwase Tracy (ID: 27105)  
**Course:** INSY 8413 – Introduction to Big Data Analytics  
**Instructor:** Eric Maniraguha  
**Date:** July 25, 2025

---

## Table of Contents

- [Executive Summary](#executive-summary)  
- [Project Overview](#project-overview)  
- [Methodology and Tools](#methodology-and-tools)  
- [Exploratory Data Analysis Highlights](#exploratory-data-analysis-highlights)  
- [Fare Changes Over Time](#fare-changes-over-time)  
- [Ride Trends by Hour, Day, Season](#ride-trends-by-hour-day-season)  
- [Seasonal and Weather Effects](#seasonal-and-weather-effects)  
- [Geographic Ride Patterns](#geographic-ride-patterns)  
- [Power BI Dashboard Design](#power-bi-dashboard-design)  
- [DAX Formulas and Measures](#dax-formulas-and-measures)  
- [Business Insights and Implications](#business-insights-and-implications)  
- [Conclusion](#conclusion)

---

## Executive Summary

This report uncovers patterns in Uber ride activity across New York City using data analysis and interactive dashboards. It applies Python for data wrangling and feature engineering, and Power BI for dashboard design and storytelling. The study investigates how temporal and spatial dimensions influence ride frequency, fare pricing, and customer demand. The final deliverable is a user-friendly Power BI dashboard offering real-time insights to support decisions in pricing, operations, and marketing.

---

## Project Overview

The dataset, sourced from Kaggle, contains ride-level Uber data across NYC. The primary objective is to surface business-relevant patterns in the data to improve operational efficiency and strategic planning.

**Key areas of analysis include:**

- Time-based fare fluctuations and demand cycles  
- Spatial hotspots of Uber activity  
- Effects of seasonal shifts on ridership  
- Identifying demand surges and underutilized periods  
- Creating actionable dashboards for real-time use

This project bridges the gap between raw data and business value, turning millions of records into clear, visual intelligence.

---

## Methodology and Tools

**Technologies Used:**

- Python (Jupyter Notebook): For data cleaning, exploration, and feature generation  
- Power BI: To design an interactive dashboard from the refined dataset  
- Libraries: `pandas`, `numpy`, `matplotlib`, `seaborn` for EDA and preprocessing

**Step-by-step Workflow:**

1. **Data Loading:** Initial CSV import using pandas  
2. **Data Cleaning:** Removing nulls, duplicates, and formatting timestamps  
3. **Outlier Detection:** Using the IQR method to exclude fare and distance outliers  
4. **Feature Engineering:** Extracting hour, weekday, month, and creating season & time-of-day labels  
5. **Visualization:** EDA charts using Python and Power BI dashboard for interactive exploration

**Data Preparation:**

![Data loading](pictures/data_loading.png)  
![Data cleaning](pictures/data_cleaning.png)

---

## Exploratory Data Analysis Highlights

The exploratory analysis focused on uncovering trends, patterns, and anomalies in the dataset. This guided the dashboard structure and business insights.

- **Fare Distribution:** Heavily right-skewed; most rides are inexpensive, but a few extreme fares exist.
- **Distance Distribution:** Most trips are under 5 km, reflecting the urban nature of NYC ride behavior.
- **Time Impact:** Clear cyclical patterns in ride demand tied to time of day and day of week.
- **Correlation:** Strong positive correlation between distance and fare, but not strictly linear due to surges and short-distance flat rates.

**EDA Visualizations:**

![EDA Histogram](pictures/eda_histogram.png)  
![EDA Boxplot](pictures/eda_boxplot.png)

---

## Fare Changes Over Time

Fare analysis focused on identifying pricing trends and demand-related spikes.

**Observations:**

- **Rush Hours:** Fares rise between 7–9 AM and 5–8 PM, consistent with commute patterns.
- **Late-Night Surges:** Weekend late-night rides often show elevated fare levels, likely due to nightlife activity and fewer available drivers.
- **Outlier Events:** Isolated spikes in fare often point to airport runs or surge pricing events (weather, demand imbalance).

**Visual Tools Used:** Line charts, boxplots, and histograms helped to isolate periods with unusual fare behavior.

![Fare Changes](pictures/fare_changes.png)

---

## Ride Trends by Hour, Day, Season

Time-of-day and calendar-based patterns are critical for workforce planning and promotions.

- **Hourly Trends:** Gradual rise in rides from early morning to peak in the evening.
- **Day-of-Week Trends:** Friday shows a surge, possibly due to work-week closure and leisure trips. Saturday and Sunday reflect late-night demand.
- **Seasonal Variation:** Spring and summer have higher ride counts, especially in afternoon and evening.

This time-based view supports scheduling and helps Uber align marketing campaigns with natural demand cycles.

![Hourly Trends](pictures/hourly_trends.png)

---

## Seasonal and Weather Effects

While real weather data was unavailable, season-based proxies helped approximate its effects.

**Insights:**

- **Spring:** Rebound in activity after winter. Tourists and outdoor mobility increase ride counts.
- **Summer:** Evening rides peak due to extended daylight, events, and tourism.
- **Autumn:** Slight decline in volume but rise in fare — suggesting longer or premium trips.
- **Winter:** Drop in early morning rides, likely due to weather deterrents or reduced commuting.

This section highlights how external context affects urban mobility patterns and supports fare prediction modeling.

![Seasonal Changes](pictures/seasonal_effects.png)

---

## Geographic Ride Patterns

Using location data, spatial trends were explored to identify zones of high and low activity.

**Key Observations:**

- High-density clusters near **Manhattan, JFK Airport**, and central business areas.
- Sparse ride density in boroughs farther from the city core.
- Indicates both opportunity for service expansion and the need for driver rebalancing strategies.

Heatmaps and geospatial visuals made it easier to pinpoint Uber’s busiest corridors and underserved regions.

![Geographic Heatmap](pictures/geographic_patterns.png)

---

## Power BI Dashboard Design

**Dashboard Title:** Tracy Uwase 27105 – Uber NYC Analysis  

The dashboard was developed to be intuitive and insight-rich, allowing users to filter by time, fare level, and location.

**Design Features:**

- **Time Filters:** Hourly, daily, monthly views  
- **Distribution Charts:** Fare and distance analysis  
- **Maps:** Visualize city zones with high/low ride frequency  
- **Slicers:** Interactive selection by season or peak/off-peak  

**User Experience Focus:**

- Easy drill-down from aggregate to specific views  
- Consistent styling for clarity  
- Ideal for executives, analysts, and operations managers

![Power BI Overview](pictures/powerbi_dashboard.png)

---

## DAX Formulas and Measures

To enhance interactivity and real-time insights in Power BI, DAX formulas were applied for dynamic aggregation.

**Custom Calculations:**

- **Time of Day Classification:** Based on hour (e.g., Morning = 5–11 AM)  
- **Season Tagging:** Spring, Summer, Autumn, Winter based on month  
- **Average Fare Metrics:** By hour, weekday, and season  
- **Peak Ride Count:** Track volume during specific time slots  
- **Dynamic Filtering:** Enabled via slicers and measures

These measures allowed the dashboard to adapt instantly to user inputs.

![DAX Measures](pictures/dax_calculations.png)

---

## Business Insights and Implications

This project translates technical results into strategic recommendations:

- **Fare Management:** Use time-based fare segmentation to increase revenue without sacrificing affordability.  
- **Driver Allocation:** Align driver shifts with peak periods and high-demand locations like airports.  
- **Customer Retention:** Offer personalized discounts during known low-volume hours.  
- **Expansion Strategy:** Use location data to identify and test new service zones.  
- **Predictive Modeling:** Build systems that forecast surge pricing windows and pre-position drivers accordingly.

These insights can help Uber reduce inefficiencies, improve rider satisfaction, and optimize operations.

---

## Conclusion

This end-to-end analysis combines Python, statistical methods, and Power BI to tell a data-driven story about Uber rides in New York City. From identifying fare surges to understanding urban demand cycles, the project equips decision-makers with actionable insights. The interactive dashboard allows ongoing exploration of trends, making this solution a valuable tool for strategic planning and operations optimization.

---


