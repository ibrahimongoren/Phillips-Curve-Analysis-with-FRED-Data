# 📊 Modern Phillips Curve Analysis with FRED Data

This repository presents a comprehensive econometric analysis of the **Modern Phillips Curve** using macroeconomic data sourced from the [Federal Reserve Economic Data (FRED)](https://fred.stlouisfed.org/). Unlike the traditional model, this version focuses on **inflation dynamics**, **inflation expectations**, and the **output gap**—excluding unemployment as an explanatory variable.

## 📌 Project Summary

The **Modern Phillips Curve** posits that current inflation is influenced by:

- Past inflation (inflation persistence)
- Expected inflation
- Real economic activity (output gap)

This notebook empirically examines the validity of this modern specification for the U.S. economy using quarterly macroeconomic data and standard econometric techniques.

---

## 📈 Key Methods and Tools

- **Python Libraries**: `pandas`, `matplotlib`, `seaborn`, `statsmodels`, `fredapi`
- **Econometric Tests**: ADF, KPSS, PP, White test, Jarque-Bera, Breusch-Pagan
- **Regression Model**: OLS (Ordinary Least Squares)
- **Diagnostic Checks**: Residual normality, heteroskedasticity, autocorrelation

---

## 🔍 Variables Used

| Variable                 | Description                                                    |
|--------------------------|----------------------------------------------------------------|
| Inflation Rate           | Current inflation rate (based on CPI)                          |
| Lagged Inflation         | One-period lag of inflation (captures persistence)             |
| Inflation Expectation    | Expected inflation (proxy via 1Y inflation breakeven or survey)|
| Real GDP                 | U.S. real GDP (seasonally adjusted, billions of chained $)     |
| Log GDP                  | Natural logarithm of real GDP                                  |
| Output Gap (%)           | % difference between actual and potential GDP                  |

**Time Period:** *Quarterly data from Q1 1982 to Q1 2024*

---

## 🧪 Model Interpretation

The OLS regression evaluates the influence of lagged inflation, expected inflation, and the output gap on the current inflation rate. Each variable reflects a theoretical aspect of price-setting behavior in modern macroeconomic models.

---
