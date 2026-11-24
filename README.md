# Crop Yield Prediction using Machine Learning

B.Tech ECE Project-1 (BECE497J), Vellore Institute of Technology, Vellore.
Team: Rithish Kumar S, Madhavan A, Vigneshwaran J. Guide: Dr. Sri Haripriya K C.

## Overview
📄 [Full project report](Crop_Yield_Prediction_Project_Report.pdf)
A machine learning model that forecasts crop yield from historical Indian crop-yield data. Accurate yield estimates help farmers, traders and policymakers plan resources, production, pricing and storage. The work supports UN SDGs 2 (Zero Hunger), 12 (Responsible Consumption and Production) and 13 (Climate Action).

## Approach
1. **Data collection:** Indian crop yield dataset (Kaggle / Directorate of Agriculture, Crops_Yield).
2. **Preprocessing and EDA:** cleaning, distribution and outlier analysis, one-hot encoding of categorical features (Crop, Season, State), train/test split.
3. **Modeling:** Random Forest Regressor and Decision Tree Regressor (scikit-learn).
4. **Evaluation:** Mean Squared Error, R-squared, residual scatter plots and predicted-vs-actual comparison.

## Results
| Metric | Random Forest | Decision Tree |
|---|---|---|
| MSE | 10346.65 | 19080.07 |
| R-squared | 0.9871 | 0.9762 |

Random Forest generalizes better because of its ensemble nature. Both models show some outliers.

## Tech stack
Python 3.12, pandas, matplotlib, seaborn, scikit-learn, Google Colab.

## Repository structure
```
├── crop_yield_prediction.ipynb   # notebook (add your Colab file here)
├── data/                         # dataset (or a link to it)
├── requirements.txt
└── README.md
```

## Run
```bash
pip install -r requirements.txt
jupyter notebook crop_yield_prediction.ipynb
```

## Future work
Hyperparameter tuning, neural networks (LSTM/GRU), satellite and remote-sensing data, interactive dashboards, and real-time weather and soil inputs.
