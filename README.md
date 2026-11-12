# Food Delivery Data Analysis

Kagnus Data Analytics Internship project. This repository holds all four weekly assignments; Week 1 (dataset understanding and cleaning) is complete.

## Project objective
Act as a junior data analyst for a food-delivery operations team: understand the delivery dataset, check its quality, clean it with every decision justified, and later explore how delivery duration varies with fields such as traffic, weather, distance, vehicle type and partner experience.

## Dataset source
Food delivery dataset supplied by Kagnus (link and access instructions in `data/raw/README.md`). The raw file is not redistributed because its licence is not stated.

## Tools and libraries
Python, Jupyter Notebook, pandas, NumPy, matplotlib, seaborn.

## Folder structure
```
food-delivery-data-analysis/
├── data/
│   ├── raw/
│   │   └── README.md                  # source and access instructions (raw CSV not uploaded)
│   └── processed/
│       └── cleaned_food_delivery.csv  # cleaned dataset (created by the notebook)
├── notebooks/
│   └── 01_data_understanding_and_cleaning.ipynb
├── docs/
│   └── cleaning_log.csv               # issue, affected column, affected rows, action, reason
├── README.md
└── requirements.txt
```

## How to run
1. Download the dataset (see `data/raw/README.md`) and save it as `data/raw/Food delivery Dataset.csv`.
2. Install the packages: `pip install -r requirements.txt`
3. Start Jupyter and open `notebooks/01_data_understanding_and_cleaning.ipynb`.
4. Run all cells from top to bottom. The notebook exports the cleaned CSV and the cleaning log and verifies that the CSV reopens correctly.

## Week 1 results
_Paste the "Week 1 summary" block printed at the end of the notebook (Section 5.1), so the numbers match your run:_

- Raw dataset: _rows x columns_. Cleaned dataset: _rows x columns_.
- Exact duplicate rows removed: _n_
- Hidden text placeholders converted to missing: _n_
- Ratings outside the assumed 0-5 scale set to missing: _n_
- Rows flagged with invalid coordinates (kept): _n_
- Most missing column after cleaning: _name, count, %_

## Assumptions and limitations
- No data dictionary was provided, so column meanings are inferred from names.
- Assumed: ratings use a 0-5 scale; plausible partner age is 18-65; valid coordinates lie in latitude 6-38, longitude 68-98.
- Missing values were not imputed; invalid coordinates were flagged, not corrected; outliers and same-ID rows with different content were kept and documented.
- Time columns have no dates, so time differences must allow for midnight.
