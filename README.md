# Global COVID-19 Analysis Dashboard

![Tableau](https://img.shields.io/badge/Tableau-Public-blue?logo=tableau)
![Dataset](https://img.shields.io/badge/Dataset-Our%20World%20in%20Data-green)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen)

## Overview

An interactive Tableau dashboard visualizing global COVID-19 trends from December 2019 to September 2020. The dashboard enables continent- and country-level exploration of cumulative cases, death tolls, and geographic distribution across 208 countries.

**Key metrics at a glance**
- Total cases: 29.90M
- Total deaths: 0.92M
- Countries tracked: 208

## Dashboard screenshot

![Global COVID-19 Dashboard](screenshot/dasboard%20screenshot.jpg)

---

## Dashboard components

### 1. Cases over time (line chart)
- Cumulative total cases plotted by month across 6 continents
- Color-encoded by continent (Africa, Asia, Europe, North America, Oceania, South America)
- Interactive date range slider (31-12-2019 to 19-09-2020)
- Continent multi-select dropdown filter

### 2. Top 10 countries by total cases (horizontal bar chart)
- Ranked bar chart with inline value labels
- Top 3: United States (6.72M), India (5.31M), Brazil (4.50M)
- Scrollable to view additional countries

### 3. Global COVID-19 cases distribution (choropleth map)
- World map colored by total cases per million population
- Sequential blue color scale (3 → 42,664 cases per million)
- Built with Mapbox + OpenStreetMap tiles

---

## Dataset

| Field | Details |
|---|---|
| Source | [Our World in Data — COVID-19](https://ourworldindata.org/covid-deaths) |
| File | `owid-covid-data.csv` |
| Date range | 31 Dec 2019 – 19 Sep 2020 |
| Granularity | Country-level, daily |
| Key columns | `location`, `date`, `continent`, `total_cases`, `total_deaths`, `total_cases_per_million` |

---

## Skills demonstrated

- Connecting to CSV data sources in Tableau
- Dimensions vs measures — date hierarchy, geographic fields
- Multi-sheet dashboard layout with shared filters
- Continent-level color encoding and legend formatting
- Choropleth map with sequential color scale
- Date range slider parameter
- KPI summary row (text objects)
- Publishing to Tableau Public

---

## How to open

1. Download [Tableau Public](https://public.tableau.com/en-us/s/download) (free)
2. Download the dataset from [Our World in Data](https://ourworldindata.org/covid-deaths)
3. Open the `.twbx` workbook file in Tableau Public
4. The data source path may need to be re-pointed to your local CSV

---

## Project structure

```
project-1-covid-dashboard/
├── README.md
├── Global_COVID19_Dashboard.twbx      # Tableau packaged workbook
├── data/
│   └── owid-covid-data.csv            # Source dataset
└── screenshots/
    └── dashboard_preview.png
```

---

## Key insights

- **North America** overtook Europe in cumulative cases by July 2020, driven by rapid US growth
- **South America** showed the steepest late-stage growth curve (June–September 2020)
- Cases per million vary dramatically — small island nations and Qatar rank highest due to population size
- Africa remained comparatively low in absolute cases but likely reflects undertesting

---

## Next steps / improvements

- Add a death rate calculated field: `[Total Deaths] / [Total Cases]`
- Replace the continent dropdown with a dashboard highlight action (click continent on map → filters line chart)
- Add a 7-day rolling average line to smooth daily fluctuations
- Include a vaccination rollout sheet once 2021 data is incorporated

---

## Author

**Sumant** — B.Tech Bioengineering, MIT-WPU Pune (2025)  
Portfolio focus: Data Science · Data Analytics · Bioinformatics  
[LinkedIn](https://www.linkedin.com/in/sumant-jadiyappagoudar/) · [Tableau Public](https://public.tableau.com/app/profile/sumant.jadiyappagoudar/vizzes) · [GitHub](https://github.com/Sumant40)

---
