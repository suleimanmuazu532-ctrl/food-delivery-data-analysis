# Raw Data

## Source
Food delivery dataset supplied by Kagnus for the Data Analytics challenge.

- File name: `Food delivery Dataset.csv`
- Access link (provided in the Kagnus project brief): https://drive.google.com/file/d/1O9WYS92iJPZoC6skyYlpcdP8Kre7eW6z/view?usp=sharing
- Size when loaded: 45,584 rows x 20 columns

## Why the raw file is not in this repository
The dataset's licence and redistribution terms were not stated in the brief, so the raw CSV is not uploaded. The original file is kept unchanged on the analyst's computer.

## How to reproduce
1. Download the file from the link above.
2. Place it in this folder (`data/raw/`) with the exact name `Food delivery Dataset.csv`.
3. Run `notebooks/01_data_understanding_and_cleaning.ipynb` from top to bottom.

The notebook never modifies the raw file. It writes the cleaned data to `data/processed/cleaned_food_delivery.csv` and the cleaning log to `docs/cleaning_log.csv`.
