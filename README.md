# Shoe Sales Revenue Predictor

A simple web app that predicts shoe sale revenue based on brand, price, units sold and other details. Built using a Random Forest model trained on 1000 shoe sales records.

## Live Demo

Open `index.html` in any browser — no installation needed.

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

## How to deploy on GitHub Pages

1. Create a new GitHub repository
2. Upload `index.html` and `README.md`
3. Go to Settings → Pages → select `main` branch → Save
4. Your app will be live at `https://yourusername.github.io/repo-name`
