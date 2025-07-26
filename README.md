# Uber-Fare-Project

Detailed Analysis Report: Uber Fares Dataset
Student: Uwase Tracy 27105  
Course: Introduction to Big Data Analytics (INSY 8413)
Instructor: Eric ManiraguhaDate: July 25, 2025

Table of Contents

Executive Summary

Project Overview

Methodology & Tools

Exploratory Data Analysis Highlights

Fare Changes Over Time

Ride Trends by Hour, Day, Season

Seasonal and Weather Effects

Geographic Ride Patterns

Power BI Dashboard Design

Business Insights and Implications

Conclusion

1. Executive Summary

This report explores the dynamics of Uber rides in New York City using data analytics and visualization. It aims to provide a high-level understanding of fare behaviors, demand fluctuations, and external influences such as time and weather proxies. The end product is an interactive that offers real-time insights for decision-makers.



2. Project Overview

The analysis began with a dataset from Kaggle containing details of individual Uber rides. This report focuses on identifying hidden patterns in:

Fare changes throughout the day and across seasons

Ride frequency by hour and weekday

Seasonal variation using time proxies

Geographic concentration of ride activity

Strategic visual storytelling via Power BI

3. Methodology & Tools

Technologies Used:

Python: For data cleaning, transformation, and feature generation

Power BI: For dynamic visualization and dashboard development

Python Libraries: pandas, numpy, matplotlib, seaborn

Analysis Steps:

Data loading and cleansing

Outlier removal using IQR

Time-based feature extraction (hour, weekday, month)

Season tagging and peak-hour flags

![Data loading](image.png)
![Data cleaning](image-1.png)

4. Exploratory Data Analysis Highlights

Before building the dashboard, a thorough exploratory data analysis (EDA) was conducted using Python to understand the structure, distribution, and relationships in the dataset.

Descriptive Statistics:

Summarized measures like average values, variation, and common trends across the dataset.

Revealed that a large portion of trips had low to moderate fare amounts and short distances.

Data Distribution and Outliers:

Fare distribution showed a clear skew with occasional very high values.

Distance data indicated a majority of short trips.

Boxplots and histograms were used to highlight extreme values and clusters.

Temporal Analysis:

Most rides took place during typical commuting hours and evenings.

Fridays and weekends showed higher demand overall.

Correlation Checks:

A visible relationship between fare and distance was observed.

Moderate patterns found between fare levels and time-of-day indicators.

This EDA phase shaped the feature engineering strategy and guided the visuals used in Power BI.

![EDA](image.png)
![EDA](image-1.png)
5. Fare Changes Over Time

General Fare Behavior:

Fares tend to concentrate around lower values but show occasional spikes associated with long-distance travel or high-demand periods.

Hourly Trends:

Fare levels increase during morning and evening commuting hours.

Slight surges may occur late at night on weekends.

Fare Distribution:

The majority of rides fall within a standard range, though outliers exist that reflect unique travel conditions.

Visualization tools like box plots helped reveal and analyze these patterns.
![Fare changes](image.png)

6. Ride Trends by Hour, Day, Season

Hourly Trends:

Ride volume steadily increases through the morning, peaking in the evening.

The quietest hours are typically between late night and early morning.

Daily Patterns:

Rides are most frequent at the end of the workweek.

Weekends reflect a shift toward late-night travel demand.

Seasonal Ride Volume:

Some seasons demonstrate higher overall activity, especially those associated with good weather or travel seasons.

Periods with extreme weather correlate with reduced ride frequency.

![Ride](image.png)
7. Seasonal and Weather Effects

Although actual weather data wasn't included, seasonal categorizations serve as a strong proxy.

Spring: A period of increased mobility, likely linked to tourism and outdoor activity.

Summer: Evening rides remain consistent due to longer daylight and social events.

Autumn: Higher average fare levels suggest changes in ride types or distances.

Winter: Reduced morning activity may reflect weather-related delays or deterrents.
![Season changes](image.png)

8. Geographic Ride Patterns

High activity in central business districts and transportation hubs.

Frequent pickups near airports and popular commercial zones.

Lower ride density in outlying boroughs and less urbanized areas.

These patterns guide efficient allocation of drivers and targeted service improvements.
![Weather effects](image.png)

9. Power BI Dashboard Design

Dashboard Name: Tracy Uwase 27105

Visual Features:

Hourly and daily ride and fare trends

Fare distribution analysis

Heatmaps for spatial and temporal clusters

Filters for key time and location dimensions

Geospatial mapping for urban demand zones

User Experience:

Highly interactive with smooth filtering and drilldowns

Designed for clarity, accessibility, and professional use

![Uber data overview](image.png)

10. DAX Formulas and Measures

To support dynamic calculations and interactivity within the Power BI dashboard, several DAX (Data Analysis Expressions) formulas were implemented:

Time-Based Measures:

Calculations to group rides by hour, day, month, and season.

Dynamic categorization of peak and off-peak periods.

Fare Aggregates:

Average fare by hour of day, day of week, and season.

Minimum and maximum fare per time block.

Custom Columns:

Time of day classification (morning, afternoon, evening, night).

Season assignment based on ride month.

Interactivity Enhancements:

Slicers controlled by DAX-based tables for clean filtering.

Measures for count of rides and total fare for selected timeframes or locations.

These calculations enhanced the user’s ability to explore patterns dynamically and supported clean, aggregated visuals in the dashboard.

![DAX](image.png)

11. Business Insights and Implications

Fare Management: Adjust pricing logic based on usage rhythms across time and season.

Driver Allocation: Prioritize driver availability in high-demand corridors and transit nodes.

Marketing Focus: Leverage downtime periods with incentives and promotions.

Geospatial Strategy: Use regional trends to uncover service gaps and areas for growth.

Forecasting Models: Build predictive systems using volume and fare trends to anticipate surges.

12. Conclusion

This detailed analysis, supported by Python and Power BI, provides actionable insights into Uber ride behavior across NYC. The study examined how time, distance, and seasons affect ride volume and fare patterns. The dashboard  enables exploration of key metrics, helping Uber teams optimize operations and enhance rider experience.
