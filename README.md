# Migraine Lifestyle Trigger Analysis

EDA project analyzing which daily lifestyle habits are associated with migraine occurrence and severity.

## Dataset
11,879 daily logs from wearable devices across 100 users. Features: sleep hours, mood, stress, hydration, screen time.

## Key Findings
- Hydration is the strongest trigger: drops from 2.88 to 2.53 on migraine days
- Clear dose-response pattern: sleep and hydration worsen as severity increases
- Migraines peak on Mondays — likely due to weekend sleep disruption
- Stress shows minimal day-level difference (contradicts common assumption)

## Tools
Python, pandas, matplotlib, seaborn

## Project Structure
- `migraine_eda.ipynb` — full analysis notebook
- `data/` — dataset
