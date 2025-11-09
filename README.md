# 🌞 Solar Challenge – Week 0

## Objective
Set up a reproducible Python environment and CI for solar radiation data analysis.

## 🌍 Project Overview

This project is part of the 10 Academy Solar Challenge (Week 0), which focuses on analyzing solar radiation and meteorological datasets from multiple African countries (Benin, Togo, Sierra Leone). The objective of Week 0 is to establish a clean, version-controlled, and reproducible environment for data profiling, cleaning, and exploratory analysis. Future weeks will extend this work into modeling and regional comparison of solar potential.


## ⚙️ Repository Structure
├── data/              # Raw and cleaned datasets (not pushed to GitHub)
├── notebooks/         # Jupyter notebooks for country-level EDA
├── scripts/           # Utility and cleaning scripts
├── reports/           # Interim and final reports, visual outputs
├── requirements.txt   # Dependencies
├── README.md          # Project documentation
└── .github/workflows/ # CI configurations


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