# Investment Morning Briefs

Static site for daily HTML morning briefs.

## Structure

- `index.html`: homepage listing all published daily briefs
- `reports/YYYY-MM-DD.html`: daily HTML reports

## Update Flow

The parent workspace script `daily_tracker.py` now:

1. Generates the local markdown and HTML report under `../reports/`
2. Copies dated HTML files into this repo under `reports/`
3. Rebuilds `index.html` so different report dates can be selected

## Publish

Use standard git commands from this repository:

```powershell
git add .
git commit -m "Publish daily morning brief"
git push origin main
```
