# 🌞 Solar Challenge – Week 0

## Objective
Set up a reproducible Python environment and CI for solar radiation data analysis.

## 🌍 Project Overview

This project is part of the 10 Academy Solar Challenge (Week 0), which focuses on analyzing solar radiation and meteorological datasets from multiple African countries (Benin, Togo, Sierra Leone). The objective of Week 0 is to establish a clean, version-controlled, and reproducible environment for data profiling, cleaning, and exploratory analysis. Additionally, conducts a cross-country comparison to identify differences in solar potential. Future weeks will extend this work into modeling and regional comparison of solar potential.


## ⚙️ Repository Structure
```
├── data/                  # Raw and cleaned datasets (not pushed to GitHub)
├── notebooks/             # Jupyter notebooks for country-level EDA and comparison
│   ├── benin_eda.ipynb
│   ├── togo_eda.ipynb
│   ├── sierraleone_eda.ipynb
│   └── compare_countries.ipynb
├── scripts/               # Utility and cleaning scripts
├── reports/               # Interim and final reports, visuals, summaries
├── requirements.txt       # Project dependencies
├── README.md              # Project documentation
└── .github/workflows/     # Continuous Integration (CI) configurations

```


## Reproduce environment (local)
1. Clone the repository:
```bash
git clone https://github.com/<YOUR_USER>/solar-challenge-week0.git
cd solar-challenge-week0
```

2. Create and activate virtual environment:
- macOS/Linux:
```bash
python -m venv venv
source venv/bin/activate
```
- Windows (PowerShell):
```bash
python -m venv venv
.\venv\Scripts\Activate.ps1
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```
4. Run future Streamlit app (example):
```bash
streamlit run scripts/app.py
```
## 🧹 Next Steps
- Complete cleaned datasets for all countries
- Begin cross-country analysis in Week 1
- Build initial data visualization dashboard using Streamlit

### Task 1 - Environment & CI Setup
- Created repository and folder structure
- Set up virtual environment and .gitignore
- Added GitHub Actions workflow for CI checks
- Documented setup process in README.md

✅ Outcome: Reproducible project setup with automated environment validation.

### Task 2 – Data Profiling & Cleaning
- Cleaned solar datasets for Benin, Togo, and Sierraleone
- Applied a consistent six-step cleaning pipeline (imputation, timestamp parsing, outlier removal, etc.)
- Conducted exploratory analysis using statistical summaries and visualizations

✅ Outcome: Clean, ready-to-analyze datasets with harmonized structures and validated metrics.

### 🌞 Task 3 – Cross-Country Comparison

- Loaded cleaned datasets and generated side-by-side boxplots for GHI, DNI, and DHI
- Computed summary statistics (mean, median, standard deviation) per country
- Performed ANOVA and Kruskal–Wallis tests to confirm significant differences