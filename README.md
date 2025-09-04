# Billionaires Dataset — Notebook README

> **Notebook file:** `LeadingIndustries.ipynb` (uploaded)

> **Dataset referenced inside notebook:** `case study - The Worlds Billionaires Dataset 1987-2022.csv`

---

## Project overview

This Jupyter notebook performs an exploratory data analysis (EDA) and deep-dive investigation of a *World's Billionaires* dataset (1987–2022). The analysis is organized around a set of business and data-science questions such as who the top billionaires are, how net worth evolved over time, which industries produced the most billionaires, nationality and demographic breakdowns, and various single-year extremes (largest net worth, steepest declines, etc.).

> **Important note:** You asked for a README for a *Leading Industries* Kaggle dataset, but the uploaded notebook actually analyzes a billionaires dataset (`case study - The Worlds Billionaires Dataset 1987-2022.csv`). If you intended a different dataset, let me know and I will re-generate README content targeted to that dataset. For now this README documents the uploaded notebook's contents.

---

## Goals & Research Questions

The notebook explicitly aims to answer (and visualise) many domain questions, including but not limited to:

* Who are the top 10 wealthiest billionaires across all years combined?
* Which billionaire had the biggest single‑year net worth?
* Who had the steepest decline in net worth in a single year?
* Which industries (sources of wealth) created the most billionaires over time?
* Trends across decades: which industry dominated each decade?
* Nationality distribution and nationality trends over time
* Demographic breakdowns (gender, age — if present in dataset)
* Time-series evolution of average/median billionaire wealth
* Special insights & interesting outliers

The notebook mixes tabular aggregation (groupby/value\_counts), filtering, ranking, and various visualization techniques to explore these questions.

---

## Notebook structure (high level)

1. **Imports & setup** — imports for `pandas`, `numpy`, `matplotlib`, `seaborn` (and any other libraries used).
2. **Data loading** — reads `case study - The Worlds Billionaires Dataset 1987-2022.csv` into a DataFrame.
3. **Initial data inspection** — `head()`, `info()`, `describe()`, missing-value checks, dtype corrections, cleaning of monetary values (e.g. converting `Networth` to numeric billions), and normalization of `Source(s) of wealth` where needed.
4. **Question-driven EDA** — a series of cells that answer the questions listed above using `groupby`, `sort_values`, `value_counts`, and time-series aggregations.
5. **Visualizations** — bar charts, line plots, heatmaps, and histograms to show distributions, trends, and comparisons over time.
6. **Findings & conclusions** — high-level takeaways from the explored questions.

---

## Key dataset columns (inferred from the notebook)

The notebook references columns including:

* `Year` — Year of the ranking/observation
* `Name` — Billionaire's name
* `Networth` — Net worth (numeric, likely in billions USD)
* `Nationality` — Country
* `Source(s) of wealth` — Industry/industries creating wealth (may be multi-valued)

If your original "Leading Industries" dataset has different column names, update the notebook accordingly.

---

## How to run this notebook locally

1. Clone or copy the notebook and the dataset file to the same folder.
2. Create and activate a Python environment (recommended):

```bash
python -m venv venv
source venv/bin/activate   # macOS / Linux
venv\Scripts\activate.bat  # Windows
pip install -r requirements.txt
```

3. Launch Jupyter:

```bash
jupyter notebook LeadingIndustries.ipynb
```

4. Run the notebook cells in order. If plots don’t render, ensure you run the plotting cells after importing matplotlib and `%matplotlib inline` (or use JupyterLab's native renderer).

---

## Required packages / `requirements.txt`

A minimal `requirements.txt` for reproducing the analysis:

```
pandas>=1.3
numpy
matplotlib
seaborn
jupyter
nbformat
```

Add extras if the notebook uses additional packages (e.g., `plotly`, `scipy`, or advanced visualization libs).

## Who are the top 10 wealthiest billionaires across all years combined?

<img width="599" height="432" alt="image" src="https://github.com/user-attachments/assets/9c0d957c-55f9-4246-af90-04f8d3126060" />

<img width="1189" height="590" alt="image" src="https://github.com/user-attachments/assets/0f1a7c4d-3dc0-4812-9c60-a92a5c229a76" />

## Which billionaire had the biggest single-year net worth?
<img width="989" height="590" alt="image" src="https://github.com/user-attachments/assets/36494cde-d5c0-4985-aeb8-adb1bfc71d2a" />

## Who had the steepest decline in net worth in a single year?

<img width="850" height="547" alt="image" src="https://github.com/user-attachments/assets/d2318546-dbe5-4680-a677-8c0e722d7bb8" />
## Which industries created the most billionaires over time?
<img width="1189" height="590" alt="image" src="https://github.com/user-attachments/assets/5b8941d7-e3eb-4268-8b2e-512f1b94f3ed" />
## Which industry dominated each decade (1980s, 1990s, 2000s, 2010s, 2020s)?
<img width="1189" height="590" alt="image" src="https://github.com/user-attachments/assets/c6ef87d9-9237-4425-ac8e-1c0b9dda14d9" />
## Co-Relation Between Age and Networth
<img width="850" height="547" alt="image" src="https://github.com/user-attachments/assets/1fb4f8fe-b717-4a8b-95f7-770f2df3acfb" />





