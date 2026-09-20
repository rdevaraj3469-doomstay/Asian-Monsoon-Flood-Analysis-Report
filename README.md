# Asian Monsoon Flood Analysis & Risk Stratification Dashboard

An end-to-end data analytics and business intelligence solution evaluating flood vulnerabilities, hydrological metrics, and environmental risk drivers across major river basins during Asian monsoon cycles[cite: 9].

---

## 📌 Project Overview

Extreme precipitation during monsoon periods presents severe ecological and socio-economic hazards across South and Southeast Asia[cite: 9]. This project processes 15,000 hydrological and environmental observations across 6 transboundary river basins to assess flood drivers, compare discharge rates, and quantify the impact of land-use changes on regional inundation risk[cite: 9].

### Core Objectives
* Clean, transform, and analyze multi-basin monsoon flood data stored in an AWS data architecture.
* Design custom DAX measures for hydrological risk assessment and event classification.
* Build an interactive executive Power BI dashboard for real-time regional risk monitoring[cite: 9].

---

## 📊 Dashboard Preview

![Asian Monsoon Flood Analysis Dashboard](docs/images/dashboard-screenshot.png)

---

## 🔍 Key Performance Indicators (KPIs)

* **Total Observations:** 15,000 historical data points across 6 basins[cite: 9].
* **Total Flood Events:** 1,000 verified flood occurrences recorded[cite: 9].
* **Average River Discharge:** 2.62K flow rate baseline[cite: 9].
* **Average Flood Probability:** 0.50 historical event likelihood baseline[cite: 9].
* **Deforestation Impact Ratio:** 2.29 runoff amplification multiplier[cite: 9].

---

## 🗺️ Monitored River Basins

The analysis covers six critical river basins:
* **Red River (`Red_River_VN`):** 207 recorded flood events (highest regional hazard)[cite: 9].
* **Chao Phraya (`Chao_Phraya_TH`):** 188 recorded flood events[cite: 9].
* **Indus Plain (`Indus_Plain_PK`):** 177 recorded flood events[cite: 9].
* **Mekong Delta (`Mekong_Delta_VN`):** 175 recorded flood events[cite: 9].
* **Ganges-Brahmaputra (`Ganges_Brahmaputra_BD`):** 172 recorded flood events[cite: 9].
* **Ayeyarwady (`Ayeyarwady_MM`):** 170 recorded flood events[cite: 9].

---

## 💡 Key Analytical Findings

1. **Urbanization Over Runoff Capacity:** Urban impervious ground consistently outpaces deforestation rates across every monitored basin, with peak coverage observed in the Red River (85K) and Chao Phraya (84K)[cite: 9].
2. **Hydrological Flow Invariance:** Average river discharge remains uniform between 2.5K and 2.7K across all basins, demonstrating that flood likelihood spikes (~0.50) are driven by sudden surface drainage saturation rather than baseflow differences[cite: 9].
3. **Upstream Deforestation Impact:** A 2.29 Deforestation Impact Ratio indicates degraded tree cover more than doubles local storm runoff speed and volume into urban centers[cite: 9].

---

## 🛠️ Tech Stack & Architecture

* **Database & Storage:** AWS S3, AWS Athena (SQL queries for aggregate metrics & filtering).
* **Business Intelligence:** Microsoft Power BI (Data Modeling, DAX, Custom Themes, KPI Tiles)[cite: 9].
* **Analytics & Preparation:** SQL / Python (Pandas) for data preprocessing.

---

## 📁 Repository Structure

```text
├── data/
│   ├── raw/                       # Raw flood and meteorological data
│   └── processed/                 # Cleaned dataset (15K rows)
├── sql/
│   ├── athena_queries.sql         # Sprint queries for metric aggregations
│   └── ddl_schema.sql             # Table definitions
├── powerbi/
│   ├── asian_monsoon_flood.pbix   # Power BI project file
│   └── dax_measures.txt           # DAX formulas for calculated columns/measures
├── docs/
│   ├── images/
│   │   └── dashboard-screenshot.png
│   └── presentation_sprint2.pdf   # Slide deck summary
└── README.md
