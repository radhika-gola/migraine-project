#1 Migraine Lifestyle Trigger Analysis

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

#2 Migraine Prediction - ML Classification Project

A end-to-end machine learning project predicting migraine occurrence from daily lifestyle data.

## Project Structure
- `migraine_eda.ipynb` — Exploratory Data Analysis
- `migraine_classification.ipynb` — ML Classification Modeling
- `data/migraine_dataset.csv` — Dataset

## Key Findings

**EDA:**
- Hydration is the strongest lifestyle predictor of migraine occurrence
- A dose-response pattern exists between sleep/hydration levels and migraine severity
- Migraines peak on Mondays

**ML Modeling:**
- Best model: Tuned Random Forest (max_depth=5) — 62% accuracy
- Hydration level accounts for ~45% of feature importance, confirming EDA findings
- Sleep hours and previous day's sleep are the next strongest predictors
- Stress level shows minimal predictive contribution across all stress features

## Models Compared
| Model | Accuracy |
|---|---|
| Logistic Regression (baseline) | 61% |
| Random Forest (untuned) | 58% |
| Random Forest (tuned, max_depth=5) | 62% |

## Tech Stack
Python, pandas, numpy, scikit-learn, matplotlib

## Conclusion
Lifestyle features show consistent predictive signal for migraines but a 62% accuracy ceiling suggests additional physiological data would be needed for clinical reliability.
