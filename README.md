# Customer Shopping Behavior — Data Analysis

Project: Exploratory analysis of customer shopping behavior using a CSV dataset and a Jupyter notebook.

Contents
- `customer_shopping_behavior.csv` — dataset used for analysis.
- `data_analysis.ipynb` — Jupyter notebook containing data loading, cleaning, feature engineering, and exploratory steps.

Overview

This repository contains an exploratory data analysis (EDA) workflow for understanding customer shopping patterns. The notebook reads the CSV, performs basic cleaning and transformations (e.g., filling missing review ratings by category median, renaming columns, creating `age_group`, mapping purchase frequency to days, and removing redundant columns), and produces summary tables for insight.

Key Notebook Steps
- Load dataset with `pandas`.
- Inspect structure with `df.head()` and `df.info()`.
- Handle missing values (example: fill `Review Rating` per `Category`).
- Normalize column names (lowercase, replace spaces with underscores).
- Create derived columns such as `age_group` and `purchase_frequency_days`.
- Drop redundant columns (for example, `promo_code_used` if identical to `discount_applied`).

Dependencies
- Python 3.8+ recommended
- pandas
- numpy
- jupyter (or JupyterLab)

Quick Start (locally)
1. Create and activate a virtual environment (optional but recommended):

   powershell
   ```powershell
   python -m venv .venv; .\.venv\Scripts\Activate.ps1
   ```

2. Install dependencies:

   powershell
   ```powershell
   pip install pandas numpy jupyter
   ```

3. Launch the notebook server and open `data_analysis.ipynb`:

   powershell
   ```powershell
   jupyter notebook
   ```

Notes & Suggestions
- The dataset `customer_shopping_behavior.csv` is included in the repository. If you prefer to keep data out of version control, add it to `.gitignore` and provide instructions to download it externally.
- Consider adding a `requirements.txt` if you want pinned dependency versions. Generate one via `pip freeze > requirements.txt` from your environment.
- Add short analysis results, visualizations, or an `outputs/` folder if you want to track generated charts (but keep large binary outputs out of Git).

License
- Add a license file (e.g., `LICENSE`) if you plan to share this repository publicly — choose an appropriate open-source license.

Contact
- If you want help extending the analysis (visualizations, modeling, or packaging), open an issue or reach out.
