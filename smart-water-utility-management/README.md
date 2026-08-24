# Smart Water Utility Management & Water Quality Intelligence-South Korea

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



### Dashboard Development Status

| Dashboard Page | Status |
|---|---|
| Page 1 — Executive Overview | ✅ Completed |
| Page 2 — Water Quality Trends | ✅ Completed |
| Page 3 — Station & Geographic Analysis | ✅ Completed |
| Page 4 — Pollution & Nutrient Analysis | 🔄 Planned |
| Page 5 — Risk & Decision Support | 🔄 Planned |

### Page 1 — Executive Overview provides a high-level view of water-quality conditions across the monitored river stations in Jeonbuk, South Korea. The page is designed to help users quickly understand the monitoring coverage, measurement volume, and overall behavior of key water-quality indicators.

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



### Page 2 — Water Quality Trends

The Water Quality Trends page focuses on understanding how key water-quality indicators change over time across the Jeonbuk river monitoring network.

The page uses time-series visualizations to help identify long-term patterns, fluctuations, and potential periods requiring further investigation.

### Indicators Analyzed

The page currently includes six time-series indicators:

| Indicator | Measure | Unit | Analytical Purpose |
|---|---|---|---|
| BOD | Average BOD | mg/L | Analyze biodegradable organic pollution trends |
| COD | Average COD | mg/L | Analyze chemical oxygen demand trends |
| DO | Average DO | mg/L | Monitor dissolved oxygen availability |
| pH | Average pH | pH units | Monitor acidity and alkalinity patterns |
| Water Temperature | Average Water Temperature | °C | Examine temperature variation over time |
| Suspended Solids | Average SS | mg/L | Analyze suspended particulate trends |

### Visualizations

The page contains six line charts:

- **BOD Trend Over Time**
- **COD Trend Over Time**
- **Dissolved Oxygen Trend**
- **pH Trend Over Time**
- **Water Temperature Trend**
- **Suspended Solids Trend**

Interactive slicers allow users to filter the analysis by:

- Year
- Season
- District
- Monitoring Station

### Key Questions

The page is designed to answer questions such as:

- How does BOD change over time?
- How does COD change over time?
- Are dissolved oxygen levels changing across the monitoring period?
- Is pH relatively stable or variable?
- How does water temperature change over time?
- Are there periods with unusually high suspended solids?
- How do these trends change when examining a specific district or monitoring station?
- Do seasonal or geographic filters reveal different patterns?

### Analytical Approach

The page uses the `Dim_Date` table for time-based analysis and the following measures:

```text
Average BOD
Average COD
Average DO
Average pH
Average Water Temperature
Average SS


### Page 3 — Station & Geographic Analysis

The Station & Geographic Analysis page focuses on identifying differences in water-quality conditions across districts and individual monitoring stations within the Jeonbuk river monitoring network.

While Page 1 provides an overall executive view and Page 2 examines temporal trends, Page 3 answers the geographic question:

> Where are differences in water-quality indicators concentrated?

The page compares average BOD, COD, Dissolved Oxygen (DO), and pH across districts and identifies monitoring stations with comparatively high average BOD.

#### Key Questions

The page is designed to answer:

- Which districts have higher average BOD levels?
- Which districts have higher average COD levels?
- How does dissolved oxygen vary across districts?
- How does pH vary across districts?
- Which monitoring stations have the highest average BOD?
- How does a selected district or monitoring station compare with the wider monitoring network?
- Do geographic filters reveal different water-quality patterns?

#### Visualizations

The page contains five primary visuals:

1. **Average BOD by District**
2. **Average COD by District**
3. **Average Dissolved Oxygen by District**
4. **Average pH by District**
5. **Top 10 Monitoring Stations by Average BOD**

#### Geographic Analysis

The district-level visuals provide a comparative view of water-quality indicators across administrative areas represented in the dataset.

BOD and COD are used to examine oxygen-demand-related pollution indicators, while DO and pH provide additional context regarding water chemistry and oxygen availability.

The analysis is descriptive and is intended to identify patterns and locations that may warrant further investigation. It does not classify a location as compliant or non-compliant without applying the appropriate water-quality standards.

#### Station-Level Analysis

The **Top 10 Monitoring Stations by Average BOD** visual provides a more detailed view of station-level variation.

The visual uses a Top N filter to identify the ten monitoring stations with the highest average BOD within the current filter context.

This allows users to move from:

```text
Regional Overview
       ↓
District Comparison
       ↓
Station-Level Investigation