# 📊 COVID-19 Visualization: Recreating NYT-style Dashboards Using Tableau

## 🎯 Project Overview

This project recreates two data visualizations originally published by *The New York Times* using COVID-19 case and death data from their public GitHub repository. The goal is to visualize pandemic trends using interactive dashboards and **advanced Tableau techniques** including:

- Table Calculations
- Trellis Maps (Small Multiples)
- Parameter Controls
- Moving Averages and Running Minimums

---

## 📂 Data Sources

- [NYT COVID-19 GitHub Repository](https://github.com/nytimes/covid-19-data)
- COVID-19 case data (up to March 2022)
- Population data by U.S. state
- State grid mapping (for trellis layout)

---

## 🛠️ Tools Used

- **Tableau Public** (Advanced visualization logic)
- **Excel** (Data preprocessing)
- **Public data** from NYT and Census Bureau

---

## 🔍 Part I – National Case Growth vs Previous Winter Peak

- Compared new COVID-19 cases from July 2021 to March 2022 against the national peak in Jan 2021.
- Created **percentage growth charts** for both Cases and Deaths.
- Used calculated fields to scale metrics and label percent changes.

📸 ![National Chart](screenshots/national_comparison_chart.png)

---

## 🗺️ Part II – State-Level Trellis Chart (Small Multiples)

- Used **parameters** and **calculated fields** (`Index`, `Row`, `Column`) to position 50 U.S. states on a grid.
- Each tile shows how the 2022 peak compares to the prior winter.
- Titles dynamically show state name and % above winter peak.

📸 ![Trellis Chart](screenshots/state_trellis_map.png)

---

## 📈 Part III – Shaded Growth Area Chart (Advanced Table Calculations)

- Used **7-day moving averages** and **running minimum** table calculations.
- Created custom logic to shade the area **after hitting the lowest case count**, indicating resurgence.
- Filtered and aligned data across time using `WINDOW_MIN()` and `RUNNING_MIN()`.

📸 ![Shaded Growth](screenshots/shaded_growth_chart.png)

---

## 💡 Key Features

| Feature                     | Technique Used            |
|----------------------------|---------------------------|
| National peak comparison   | Aggregated filtering      |
| State comparison           | Trellis grid layout       |
| Shaded resurgence area     | Nested table calculations |
| Dashboard storytelling     | Tableau formatting        |

---

## 📁 Folder Structure

