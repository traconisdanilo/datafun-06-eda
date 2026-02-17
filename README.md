# datafun-06-eda

Foundations of Data Analytics, Module 6. Custom EDA Project.

**Author:** Danilo Traconis  
**Date:** February 16, 2026  
**Purpose:** Perform exploratory data analysis (EDA) on a dataset using Jupyter, pandas, matplotlib, and seaborn.

---

## Initial Setup

1. Created this repository on GitHub with a default README.
2. Opened the `Repos` folder from the C: drive in Windows PowerShell.
3. Cloned the repository to my machine using:

```powershell
git clone https://github.com/traconisdanilo/datafun-06-eda
```

4. Navigated into the project folder and opened it in VS Code:

```powershell
cd datafun-06-eda
code .
```

5. Added `.gitignore` and `requirements.txt` with standard Python project settings.
6. Used Git to add, commit, and push changes to GitHub.
7. Enabled GitHub Actions and Dependabot security updates in repository settings.

---

## Virtual Environment Setup

8. Verified Python installation from python.org and ensured:
   - Add Python to PATH was checked
   - Add Python to environment variables was enabled

9. Created the project virtual environment:

```powershell
python -m venv .venv
```

10. Activated the virtual environment:

```powershell
.\.venv\Scripts\Activate
```

11. Upgraded pip, setuptools, and wheel:

```powershell
python -m pip install --upgrade pip setuptools wheel
```

12. Installed required project dependencies:

```powershell
python -m pip install -r requirements.txt
```

13. Verified installation by successfully importing numpy, pandas, pyarrow, matplotlib, and seaborn.

14. Created an initial Jupyter notebook and starter script for EDA.

---

## Reminder

Each time you open a new PowerShell session for this project, activate the virtual environment before running Python commands:

```powershell
.\.venv\Scripts\Activate
```

If needed, confirm dependencies are installed:

```powershell
python -m pip install -r requirements.txt
```

---

## Commands Used

```powershell
git clone https://github.com/traconisdanilo/datafun-06-eda
cd datafun-06-eda
code .

git add .
git commit -m "Project initialization"
git push -u origin main

python -m venv .venv
.\.venv\Scripts\Activate

python -m pip install --upgrade pip setuptools wheel
python -m pip install -r requirements.txt
```

---

## Dataset Description (CC6.2)

**Dataset Name:** Student Academic Stress Level Dataset  

**Source (Kaggle):**  
https://www.kaggle.com/code/alkatsir/student-stres-level/notebook  

**Number of Records:**  
140 survey responses  

**Number of Columns:**  
9 original columns  

### Column Descriptions

| Column Name | Description |
|-------------|-------------|
| Timestamp | Date and time the survey was submitted |
| Your Academic Stage | Education level (high school, undergraduate, post-graduate) |
| Peer pressure | Self-rated peer pressure (1–5 scale) |
| Academic pressure from your home | Family academic pressure (1–5 scale) |
| Study Environment | Type of study environment (Peaceful, Noisy, Disrupted) |
| What coping strategy you use as a student? | Main stress coping method |
| Do you have any bad habits like smoking, drinking on a daily basis? | Yes / No / Prefer not to say |
| What would you rate the academic competition in your student life | Academic competition level (1–5 scale) |
| Rate your academic stress index | Self-rated stress level (1–5 scale) |

### Purpose of Dataset in This Project

This dataset will be used to explore relationships between academic stage, pressure sources, coping strategies, habits, and overall academic stress levels. The goal is to identify patterns and visualize factors that may contribute to higher student stress levels.
