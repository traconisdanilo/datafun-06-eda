# datafun-06-eda

## Project Initialization Notes

## Commands Used

```powershell
cd C:\Repos
git clone https://github.com/YOUR-USERNAME/datafun-06-eda.git
cd datafun-06-eda

python --version
python -m venv .venv
.\.venv\Scripts\Activate

python -m pip install --upgrade pip setuptools wheel
python -m pip install -r requirements.txt

python -c "import numpy, pandas, pyarrow, matplotlib, seaborn; print('all imports ok')"
python scripts/eda.py
