# Smart Water Utility Management & Water Quality Intelligence
# Smart Water Utility Intelligence Dashboard — South Korea

An interactive business intelligence project analyzing
water-quality monitoring data from Jeonbuk, South Korea.

## Project Objective

The project transforms official Korean water-quality monitoring
data into an interactive Power BI decision-support dashboard.

The dashboard aims to help users understand water-quality trends,
compare monitoring stations, identify potential high-risk areas,
and support data-driven environmental decisions.

## Business Questions

- Which monitoring stations have the highest water-quality risk?
- How does water quality change over time?
- Which parameters show deterioration?
- Are there seasonal patterns?
- Which locations require further investigation?
- Which water-quality indicators contribute most to risk?

## Dataset

The raw dataset is stored in:

`data/raw/`

## Technology

- Microsoft Power BI
- Power Query
- DAX
- Python
- GitHub

## Project Structure

```text
data/            → Raw and processed datasets
documentation/   → Business and analytical documentation
powerbi/         → Power BI dashboard files and screenshots
python/          → Data profiling and analysis
dax/             → DAX measures
images/          → Project visuals




Executive Overview

Page 1 — Executive Overview provides a high-level view of water-quality conditions across the monitored river stations in Jeonbuk, South Korea. The page is designed to help users quickly understand the monitoring coverage, measurement volume, and overall behavior of key water-quality indicators.

The dashboard summarizes Biochemical Oxygen Demand (BOD), Chemical Oxygen Demand (COD), Dissolved Oxygen (DO), and pH, while allowing users to filter results by year, season, district, and monitoring station.

Key questions answered
How many monitoring stations are represented in the dataset?
How many water-quality measurements are available?
What are the average BOD, COD, DO, and pH levels?
How have BOD, COD, and DO changed over time?
Which monitoring stations have the highest average BOD?
Which districts show higher average BOD levels?
How do the results change when filtering by year, season, district, or station?
Main dashboard components
Component	Purpose
Monitoring Stations	Shows the number of unique monitoring stations
Total Measurements	Shows the number of records available
Average BOD	Summarizes biodegradable organic pollution demand
Average COD	Summarizes chemical oxygen demand
Average DO	Shows dissolved oxygen availability
Average pH	Shows the overall acidity/alkalinity indicator
BOD Trend	Examines BOD changes over time
COD Trend	Examines COD changes over time
DO Trend	Examines dissolved oxygen changes over time
Top 10 Stations by Average BOD	Identifies stations requiring further investigation
Average BOD by District	Compares geographic variation
Slicers	Enables year, season, district, and station-level exploration
