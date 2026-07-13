# Barbourville EV Charging Dashboard

Interactive benchmark dashboard analyzing 12 months of public EV charging data from Barbourville, KY (BARBOURVILLE / CITY HALL Level 3 DCFC and BARBOURVILLE / TOURISM Level 2 chargers). Built as a benchmark exhibit for Pineville, KY, which is considering installing its own Level 2 charger.

**Live dashboard:** https://irumvaa.github.io/barbourville-ev-dashboard/

## Contents
- `index.html`: self-contained interactive dashboard (Chart.js + Leaflet, no external dependencies needed to run). Includes:
  - Overview, Usage Patterns, Visitor Origin & Map, Financial, and For the City tabs
  - A station toggle (Combined / Tourism Level 2 / City Hall Level 3) that filters KPIs, charts, and tables throughout
  - Sessions by time of day, day of week, per day, and per week
  - A Leaflet map of driver origin that shows state-level markers by default and switches to county-level markers on zoom
  - A full financial reconciliation panel per station, including a 15-row sample table that always surfaces the one flagged (non-reconciling) session
- `Barbourville_EV_Charging_Analysis.xlsx`: full Excel workbook, fully formula-driven throughout. Includes:
  - Dashboard, Tourism (Level 2), and City Hall (Level 3) summary tabs
  - Daily Summary, Time of Day, and Frequency & Day of Week tabs
  - Revenue & Economic Impact tab with a live monthly trend
  - Financial Reconciliation tab: a live 288-row check of every session's Gross Amount and Payout Amount against the raw fee/tax columns, with conditional formatting and an autofilter to isolate any flagged rows
  - Visitor Origin and Net Zero & Recommendations tabs
  - Raw data tabs that every formula in the workbook traces back to, so editing a raw value updates every dependent table, KPI, and sentence automatically

## Data sources
ChargePoint dashboard exports (Sessions, Charging Session Updates, Organization Statement, Energy-vs-Time), Barbourville City Tourism account, Jul 2025 to Jul 2026.

Prepared by a Mountain Association Energy Intern. Internal benchmark exhibit, not an official city economic study.
