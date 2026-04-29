# Shoe Sales Revenue Predictor

A simple web app that predicts shoe sale revenue based on brand, price, units sold and other details. Built using a Random Forest model trained on 1000 shoe sales records.

## Live Demo

[Demo](https://mohdsaqib19.github.io/Shoe-Sales-Revenue-Predictor/)

## How it works

You fill in:
- Brand (Nike, Adidas, Puma, etc.)
- Shoe type, color, country
- Sales channel (Online, Mall, Retail)
- Price and units sold

Click **Predict** and it shows the estimated revenue instantly.

## Model Info

| Model | R² Score | MAE |
|-------|----------|-----|
| Linear Regression | 0.8994 | $267 |
| **Random Forest** | **0.9978** | **$37** |
| Gradient Boosting | 0.9979 | $38 |

Random Forest was selected as the final model. The two most important features are `Price_USD` and `Units_Sold` which together account for ~99% of the prediction.

The model was trained in Python (scikit-learn) and the prediction logic is converted to JavaScript so it runs directly in the browser without any backend.

## Files

```
index.html      - main web app
README.md       - this file
```

## Dataset

1000 shoe sales records with columns: Brand, Shoe Type, Color, Country, Sales Channel, Price, Units Sold, Revenue.

## Tech Used

- HTML, CSS, JavaScript (frontend)
- Python + scikit-learn (model training)
- Random Forest Regressor

## How to run locally

Just download `index.html` and open it in your browser. That's it.

