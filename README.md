# Kenya Refugee & Asylum-Seeker Population Dashboard

An interactive Power BI dashboard analyzing Kenya's registered refugee and asylum-seeker population, built from UNHCR's official statistics.
## Dashboard Preview

![Kenya Refugee and Asylum-Seeker Population Dashboard](dashboard-screenshot.png)

**Live dashboard:** https://app.powerbi.com/view?r=eyJrIjoiMDFlMzU0NzgtNWIzMS00ZWNiLThiMzItMWNhZjM4ODM5NWViIiwidCI6ImRmODY3OWNkLWE4MGUtNDVkOC05OWFjLWM4M2VkN2ZmOTVhMCJ9

## Overview

This project visualizes population trends, demographics, and registration activity for refugees and asylum-seekers hosted in Kenya, using UNHCR's Kenya Statistics Package (as of 31 August 2026). The dashboard was built end-to-end: source data cleaning, data modeling, and interactive visualization.

## Data Source

- **UNHCR Kenya Statistics Package**, 31 August 2026
- Published by UNHCR Kenya — DIMA Unit, Nairobi
- Source: [data.unhcr.org/en/country/ken](https://data.unhcr.org/en/country/ken)

The original PDF statistics package was reshaped into clean, tidy tables (Year/Location/Population format) before loading into Power BI, since the source PDF's multi-level headers and merged cells were not directly machine-readable.

## Tools Used

- **Power BI Desktop** — data modeling and visualization
- **Power Query** — data cleaning and shaping
- **DAX** — KPI measures
- **Power BI Service** — publishing (Publish to Web)

## Dashboard Contents

- **KPI cards:** Total registered population, % women & children, % living in camps, refugees vs. asylum-seekers
- **Population by location** (bar chart, 2026)
- **5-year population trend by location** (2022–2026, line chart)
- **Population by country of origin** (stacked bar, 2022–2026)
- **Monthly 2026 registration trend** by location
- **Demographics by age group and gender** (clustered bar chart)
- **Year slicer** for interactive filtering

## Key Findings

- **Dadaab hosts the largest and fastest-growing population** — 429,352 as of August 2026, with registrations climbing sharply from April 2026 onward, far outpacing other locations.
- **Somalia is the dominant country of origin**, consistently representing roughly 55% of the total population across the full 2022–2026 trend, followed by South Sudan.
- **The working-age group (18–59) is the largest demographic segment**, making up approximately 46% of the total population.
- Total registered population grew from **573,508 in 2022 to 871,568 in 2026**, with a notable plateau between 2024 and 2025 before climbing again into 2026.

## Notes

- The **Year slicer** filters the location trend, 5-year trend, and country-of-origin charts, since those tables include a Year field. It does **not** affect the four KPI cards, which are fixed snapshot figures as of 31 August 2026 (sourced from a separate summary table with no Year dimension) — this is expected behavior, not a bug.
- All figures are sourced directly from UNHCR's published statistics; no figures were estimated or modeled.

## Author

Margaret Wanjiku Wanjiru
[LinkedIn] • [GitHub: margaretwanjiku438-oss](https://github.com/margaretwanjiku438-oss)
