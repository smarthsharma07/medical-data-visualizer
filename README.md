# medical-data-visualizer
# Medical Data Visualizer

This project analyzes and visualizes medical examination data using **Python, Pandas, Matplotlib, and Seaborn**.  
It is part of the **freeCodeCamp Data Analysis with Python** certification.

The goal is to explore relationships between cardiovascular disease, body measurements, blood markers, and lifestyle choices through data cleaning, feature engineering, and visualization.

---

## Dataset

- **File:** `medical_examination.csv`
- **Source:** Medical examination data (provided by freeCodeCamp)
- **Rows:** Patients
- **Columns:** Medical measurements, lifestyle indicators, and cardiovascular disease status

### Key Features
- Age (in days)
- Height (cm), Weight (kg)
- Blood pressure (systolic & diastolic)
- Cholesterol & glucose levels
- Lifestyle indicators (smoking, alcohol, physical activity)
- Cardiovascular disease indicator (`cardio`)

---

## Project Objectives

The project performs the following tasks:

### 1. Data Preparation
- Add an `overweight` column using BMI calculation
- Normalize cholesterol and glucose values:
  - `0` → good
  - `1` → bad

### 2. Categorical Plot
- Visualize counts of health and lifestyle indicators:
  - cholesterol, glucose, smoking, alcohol intake, physical activity, overweight
- Compare outcomes for patients **with** and **without** cardiovascular disease
- Uses data reshaping (`pd.melt`) and aggregation

### 3. Heat Map
- Clean incorrect or extreme data points
- Compute correlation matrix
- Visualize correlations using a masked heat map

---

## Technologies Used

- Python 3
- Pandas
- NumPy
- Matplotlib
- Seaborn
- unittest (for automated testing)

---

## Project Structure

```
├── medical_data_visualizer.py # Main analysis and plotting logic
├── main.py # Local test runner
├── test_module.py # Unit tests (provided by FCC)
├── medical_examination.csv # Dataset
└── README.md
```
