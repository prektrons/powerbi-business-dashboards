# Methodology

## 1. Data Source

The project uses official South Korean water-quality monitoring
data for Jeonbuk.

The original source file is stored in:

`data/raw/`

The raw dataset will remain unchanged.

## 2. Data Pipeline

The analytical workflow will follow:

Raw Data
    ↓
Data Profiling
    ↓
Data Quality Assessment
    ↓
Data Cleaning
    ↓
Data Transformation
    ↓
Data Modeling
    ↓
Power BI
    ↓
DAX Measures
    ↓
Dashboard
    ↓
Risk Analysis

## 3. Analytical Dimensions

The analysis will consider:

- Time
- Monitoring station
- Geographic location
- Water-quality parameters
- Seasonal patterns

## 4. Water-Quality Indicators

The project will analyze available parameters including:

- Water temperature
- pH
- Dissolved Oxygen (DO)
- Biochemical Oxygen Demand (BOD)
- Chemical Oxygen Demand (COD)
- Suspended Solids (SS)
- Total Nitrogen (TN)
- Total Phosphorus (TP)
- Total Organic Carbon (TOC)

The final list will be confirmed after profiling the actual
CSV dataset.

## 5. Dashboard Approach

The Power BI dashboard will use:

- KPI cards
- Time-series charts
- Station rankings
- Parameter comparisons
- Geographic visualization
- Trend analysis
- Risk indicators

## 6. Risk Analysis

A water-quality risk score may be introduced after the baseline
dashboard has been developed.

The risk methodology will be documented separately and will be
based on available water-quality indicators and appropriate
thresholds.

## 7. Data Quality

Before visualization, the dataset will be assessed for:

- Missing values
- Duplicate records
- Invalid values
- Data types
- Outliers
- Inconsistent station names
- Missing dates
- Measurement anomalies
