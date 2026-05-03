# Berkeley-AI-Program-Capstone-Project-
# What Drives the Price of a Used Car?

## Project Overview
This project analyzes a dataset of approximately 426,000 used cars to understand the key factors that influence vehicle pricing. The goal is to help a used car dealership make better inventory and pricing decisions by identifying what consumers value most in a used vehicle.

Using the CRISP-DM framework, this project includes data cleaning, exploratory data analysis, feature engineering, and predictive modeling.

---

## Business Problem
A used car dealership wants to understand:
- What factors most strongly influence car prices?
- Which features increase or decrease resale value?
- How can they optimize inventory selection for profitability?

---

## Dataset
- Source: Kaggle Used Cars Dataset
- File used: `vehicles.csv`
- Records: ~426,000 used car listings

---

## Key Findings

### Factors that Increase Price:
- Newer vehicle year
- Lower mileage (odometer)
- Luxury brands (BMW, Lexus, Mercedes-Benz, etc.)
- Good/excellent condition
- Clean title status

### Factors that Decrease Price:
- High mileage
- Older vehicles
- Salvage or rebuilt titles
- Poor condition ratings

---

## Modeling Approach
Multiple regression models were tested:
- Linear Regression
- Ridge Regression
- Random Forest Regressor

### Best Performing Model:
- Random Forest Regressor
- Provided highest predictive accuracy and best generalization

### Evaluation Metrics:
- RMSE (Root Mean Squared Error)
- MAE (Mean Absolute Error)
- R² Score

---

## Recommendations for Dealership

1. Prioritize inventory with **low mileage and newer model years**
2. Focus on **reliable, high-demand brands**
3. Avoid high-mileage older cars unless heavily discounted
4. Use model-based pricing estimates to reduce overpricing/underpricing
5. Invest more in vehicles with clean titles and good condition ratings

---

## Files in Repository
- `notebook.ipynb` → Full analysis and modeling
- `README.md` → Project summary (this file)

---

## How to Run This Project
1. Clone repository
2. Ensure `vehicles.csv` is in project folder
3. Install dependencies:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
