# Predictive Analytics Examination – Air Quality Forecasting

This repository contains my **PGR304** **Predictive Analytics** exam at Kristiania University College. It explores how **Vector Autoregression (VAR)** and **Seasonal ARIMA with exogenous regressors (SARIMAX)** forecast three pollutants—**CO**, **NO₂**, and **relative humidity**—from the [UCI Air Quality dataset](https://archive.ics.uci.edu/dataset/360/air+quality).

The notebooks show the full pipeline: cleaning, exploratory analysis, lag‑order and hyper‑parameter search, model fitting, and diagnostics. A cached grid‑search of optimal SARIMAX settings lives in `<span>best_sarimax_parameters.csv</span>`; the workflows themselves are in `<span>VAR.ipynb</span>` and `<span>SARIMAX.ipynb</span>`. The written rationale, figures, and results are summarised in `<span>Predictive_Analytics_Exam_Report.pdf</span>`, where VAR proved best for RH while SARIMAX edged ahead on CO and NO₂.

## Use

1. Download the UCI dataset from their webpage and save it to the folder where the notebooks are found.`<span>pip install -r requirements.txt</span>`
2. Open the notebooks and run all cells (or adapt them into scripts).
3. To rerun the SARIMAX grid search, tweak the search space in the first cell of `<span>SARIMAX.ipynb</span>`.

Tested on Python 3.11 with Statsmodels, pandas, scikit‑learn, and Matplotlib.
