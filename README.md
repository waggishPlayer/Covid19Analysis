# COVID-19 Trend Analysis

This project analyzes historical COVID-19 case data using a Jupyter notebook.
It performs basic cleaning, aggregation, and visualization of confirmed, deaths, and recovered counts by country and over time.

## Repository Contents

- `covid-19_trendAnalysis.ipynb` - main analysis notebook
- `covid_19_data.csv` - input dataset used by the notebook

## What the Notebook Does

1. Loads COVID-19 data from `covid_19_data.csv`
2. Drops unused columns (`SNo`, `Last Update`)
3. Renames columns for easier use:
   - `ObservationDate` -> `Date`
   - `Province/State` -> `State`
   - `Country/Region` -> `Country`
4. Converts `Date` to datetime
5. Applies missing-value imputation
6. Aggregates data by:
   - `Country` and `Date`
   - global totals by `Date`
7. Generates scatter plots showing trends of Confirmed, Recovered, and Deaths

## Requirements

Install Python packages used in the notebook:

- `jupyter`
- `pandas`
- `numpy`
- `matplotlib`
- `scikit-learn`

Example install:

```bash
pip install jupyter pandas numpy matplotlib scikit-learn
```

## How to Run

1. Clone the repository.
2. Open terminal in the project directory.
3. Start Jupyter:

```bash
jupyter notebook
```

4. Open `covid-19_trendAnalysis.ipynb`.
5. Run all cells in order.

## Notes

- The notebook expects `covid_19_data.csv` to be in the same directory.
- Visualizations are generated directly in notebook cells.
