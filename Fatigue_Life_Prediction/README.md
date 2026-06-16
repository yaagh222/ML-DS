# ML-Based Fatigue Life Prediction of a Stepped Shaft

## Overview
A machine learning project that predicts the minimum fatigue life 
of a stepped shaft using simulation data generated from ANSYS 
Mechanical. Bridges mechanical engineering simulation with 
data-driven modelling.

---

## Workflow
1. **Simulation** — Designed a parametric stepped shaft in ANSYS 
   Mechanical with stress concentration zones. Ran fatigue analysis 
   using Goodman mean stress theory and S-N curve (Stress Life).
2. **Data Generation** — Used Latin Hypercube Sampling to generate 
   100 design points across varying shaft geometry and load parameters.
3. **EDA & Profiling** — Cleaned and explored simulation data using 
   Pandas and Matplotlib.
4. **Modelling** — Built Linear Regression and Random Forest models 
   using Scikit-learn to predict minimum fatigue life.

---

## Results
| Model | R² Score |
|---|---|
| Linear Regression | 0.624 |
| Random Forest | 0.624 |

> Dataset size: 100 simulation points (ANSYS solve time was the 
> limiting factor for dataset size)

---

## Tools & Libraries
- ANSYS Mechanical (fatigue simulation)
- Python, Pandas, Matplotlib
- Scikit-learn

---

## Files
| File | Description |
|---|---|
| `DesignPointLog2.csv` | Raw simulation output |
| `MinimumLife_Data.csv` | Cleaned dataset |
| `MinimumLife_DataCleaning.ipynb` | Data cleaning |
| `MinimumLife_EDA.ipynb` | Exploratory analysis |
| `MinimumLife_Profiling.ipynb` | Data profiling |
| `MinimumLife_Prediction.ipynb` | ML models |
| `FatigueLoading_Report.html` | Profiling report |
