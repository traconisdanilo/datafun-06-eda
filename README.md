# datafun-06-eda

Exploratory Data Analysis: Student Academic Stress Level  
Foundations of Data Analytics, Module 6. Custom EDA Project.

**Author:** Danilo Traconis  
**Date:** February 16, 2026  
**Purpose:** Perform exploratory data analysis (EDA) on a student stress survey dataset using Jupyter, pandas, matplotlib, and seaborn.

---

## Dataset Description

**Dataset:** Student Academic Stress Level Dataset  
**Source:** Kaggle Notebook — Student Stress Level  
https://www.kaggle.com/code/alkatsir/student-stres-level/notebook  

**Records:** 140 survey responses  
**Columns:** 9

### Column Descriptions

| Column | Description | Type |
|---|---|---|
| Timestamp | Date/time the survey was submitted | Time |
| Your Academic Stage | Education level (high school, undergraduate, post-graduate) | Categorical |
| Peer pressure | Self-rated peer pressure (1–5 scale) | Numeric |
| Academic pressure from your home | Family/home academic pressure (1–5 scale) | Numeric |
| Study Environment | Study environment category (Peaceful, Noisy, disrupted) | Categorical |
| What coping strategy you use as a student? | Primary coping strategy | Categorical |
| Do you have any bad habits like smoking, drinking on a daily basis? | Yes / No / Prefer not to say | Categorical |
| What would you rate the academic competition in your student life | Academic competition rating (1–5 scale) | Numeric |
| Rate your academic stress index | Overall academic stress index (1–5 scale) | Numeric |

**Note on missing data:** The raw dataset contains 1 missing value in `Study Environment`. For analysis, I will either drop missing rows or fill missing values (documented in the notebook).

---

## Initial Setup

- Created this repository on GitHub with a default `README.md`.
- Opened the `Repos` folder from the C: drive in Windows PowerShell and cloned the repo.
- Opened the project in VS Code (`code .`).
- Added `.gitignore` and `requirements.txt` with standard Python project settings.
- Used Git to add, commit, and push updates to GitHub.
- Enabled GitHub Actions and Dependabot security updates in repository settings.

---

## Virtual Environment Setup (Windows 11 PowerShell)

Verified Python installation from python.org and ensured:
- ✅ Add Python to PATH
- ✅ Add Python to environment variables

Created and activated the project virtual environment:

```powershell
python -m venv .venv
.\.venv\Scripts\Activate
```

Upgraded core packaging tools and installed dependencies:

```powershell
python -m pip install --upgrade pip setuptools wheel
python -m pip install -r requirements.txt
```

Verified imports:

```powershell
python -c "import numpy, pandas, pyarrow, matplotlib, seaborn; print('all imports ok')"
```

---

## Project Structure

- `data/` — local dataset storage (not pushed to GitHub)
- `scripts/` — helper scripts (e.g., quick checks)
- `*.ipynb` — the EDA notebook (created in project root)

---

## Notebook Overview

The notebook will follow an 8-step EDA workflow:

1. **Data Acquisition** — Load the CSV into a pandas DataFrame.
2. **Initial Data Inspection** — Preview rows, check shape, dtypes, missing values.
3. **Descriptive Statistics** — Summaries for numeric and categorical columns.
4. **Numerical Distributions** — Histograms/boxplots for rating columns.
5. **Categorical Distributions** — Count plots for academic stage, environment, coping, habits.
6. **Transformation & Feature Engineering** — Rename at least one column and add at least one new column (e.g., `total_pressure` or `stress_level_group`).
7. **Visualizations & Questions** — At least 3 chart/story sections (goal → chart type → chart → story).
8. **Storytelling & Presentation** — Summarize results clearly and visually.

---

## Key Questions (Planned)

- Do students reporting higher **peer pressure** also report higher **stress index**?
- Does **study environment** (Peaceful vs Noisy vs disrupted) relate to stress?
- Do certain **coping strategies** cluster with higher stress ratings?
- How does **academic stage** (high school vs undergraduate vs post-graduate) differ in stress?

---

## Key Findings (To Be Updated)

This section will be updated after completing the notebook analysis. Example items may include:
- The strongest factor associated with high stress.
- Differences in stress levels by academic stage.
- Most common coping strategies and how they vary by stress level.

---

## Reminder

Each time you open a new PowerShell session for this project, activate the virtual environment before running Python or Jupyter commands:

```powershell
.\.venv\Scripts\Activate
```

If needed, reinstall dependencies:

```powershell
python -m pip install -r requirements.txt
```

---

## Commands Used

```powershell
git clone https://github.com/traconisdanilo/datafun-06-eda
cd datafun-06-eda
code .

python -m venv .venv
.\.venv\Scripts\Activate
python -m pip install --upgrade pip setuptools wheel
python -m pip install -r requirements.txt

git add .
git commit -m "Descriptive message"
git push
```

