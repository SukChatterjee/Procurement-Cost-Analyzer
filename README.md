# BOM Cost Optimizer (Excel + Python + SQL)

A small procurement analytics toolkit to estimate build cost, compare vendors, and validate pricing data.
Built to mimic how operations teams do quick sourcing decisions: spreadsheet-first, then script/SQL checks.

## Key features
- **Vendor price catalog**: multiple vendor price lists per part
- **BOM costing**: total quantity + extended cost + grand total for a build
- **Vendor comparison**: switch vendors and instantly see the total cost change
- **Data quality checks** (Python/SQL):
  - missing price detection
  - duplicate Part_ID checks
  - inconsistent part naming checks
- **What-if ready**: change build quantity and see cost impact

## Project structure
- `excel/` → pricing catalog + BOM cost model
- `python/` → export summaries + run validation checks
- `sql/` → schema + analytics queries (rollups, missing prices, vendor totals)
- `screenshots/` → quick visuals for reviewers

## Why this exists
In real projects, analysts often start in Excel to align with stakeholders,
Then use Python/SQL to validate logic and automate reporting.
This repo demonstrates an end-to-end workflow in a compact format.

## Notes
All data is synthetic and for demonstration only.
