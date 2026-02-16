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

