# Opt_Group Project

## Environment

- **Conda environment:** `project`
- **Activate:** `conda activate project`
- All packages must be installed into this environment
- Key packages (see `requirements.txt`): numpy, scipy, pandas, cvxpy, pulp, matplotlib, seaborn, jupyter, ipykernel, tqdm

## Project Description

**IEOR E4004 Spring 2026 — Course Project I**
**Topic:** Eliminating Child Care Deserts in New York City through Optimization

### Desert Classification

- **High-demand area** (employment ≥ 60% OR avg income ≤ $60k): desert if slots ≤ 0.5 × children pop (ages 0–12)
- **Normal-demand area**: desert if slots ≤ 1/3 × children pop (ages 0–12)
- **NYC policy**: slots for ages 0–5 must be ≥ 2/3 × pop aged 0–5

### Problem I — Idealistic Budgeting

**Goal:** Minimize total funding to eliminate childcare deserts in every NYC zipcode.

- Can build new facilities anywhere from candidate locations
  - Small: $65k / 100 slots
  - Medium: $95k / 200 slots
  - Large: $115k / 400 slots
- Can expand existing facilities up to 120% of current capacity or +500 slots (whichever is binding)
- Piecewise expansion cost per slot `x_f` at facility `f` with current capacity `n_f`:
  - If `x_f < n_f`: `c_slots(n_f) * x_f`
  - If `x_f ≥ n_f`: `(20000 + 200*n_f) * x_f / n_f`
- Extra $100/slot for children under age 5

### Problem II — Realistic Scenario

**Goal:** Minimize cost subject to tighter constraints.

- Expansion capped at 20% of current capacity
- Piecewise increasing marginal expansion cost:
  - 0–10%: `(20000 + 200*n_f) * x_f / n_f`
  - 10–15%: `(20000 + 400*n_f) * x_f / n_f`
  - 15–20%: `(20000 + 1000*n_f) * x_f / n_f`
- Distance constraint: no two facilities within 0.06 miles of each other

## Data Files (`data/raw/`)

| File | Description |
|---|---|
| `child_care_regulated_nyc.csv` | Existing facilities (7,740 rows) |
| `population_nyc.csv` | Population by age group per zipcode |
| `avg_individual_income_nyc.csv` | Avg income per zipcode |
| `employment_rate_nyc.csv` | Employment rate per zipcode |
| `potential_locations_nyc.csv` | Candidate locations for new facilities |

## Main Notebook

`notebooks/childcare_optimization.ipynb`
