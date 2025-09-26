# Forecasting-housing-price-index
"This project analyzes the U.S. Housing Price Index (1991–2013) using time series methods. After cleaning and enhancing the dataset with economic variables, we applied SARIMA and SARIMAX models. The SARIMA(1,1,1)(0,1,1) model provided the best forecast accuracy, capturing both trend and seasonality."
📌 Project Overview

This project analyzes the U.S. Housing Price Index (HPI) from 1991 to 2013 using advanced time series modeling. The goal was to forecast housing prices, assess the impact of the 2007 housing crash, and evaluate the influence of external economic variables.

🗂 Dataset

Source: U.S. Housing Price Index (monthly data, 1991–2013)

Variables:

HPI – Housing Price Index (target variable)

numsold – Number of houses sold (in thousands)

fedfunds – Federal funds rate (added from research)

event – Dummy variable for the 2007 housing crash (0 before, 1 after)

🔍 Methodology

Data Preprocessing

Imputed missing dates using monthly patterns

Integrated macroeconomic variables (federal funds rate, event dummy)

Exploratory Analysis

Raw series visualization showing growth, crash, and recovery

Time series decomposition: trend, seasonality, residuals

Modeling

Tested multiple SARIMA and SARIMAX models

Compared models using AIC, SBC, RMSE, and MAPE

Performed residual diagnostics for autocorrelation

📊 Key Findings

Housing Price Index shows strong trend + seasonal patterns

Cross-correlation:

numsold follows HPI

fedfunds leads HPI inversely

Best Model: SARIMA(1,1,1)(0,1,1)

MAPE: 0.38%

RMSE: 0.99

Captured both trend and seasonality effectively

✅ Conclusion

The 2007 housing crash introduced structural breaks and volatility.

Adding exogenous variables did not significantly improve forecasting accuracy.

Future directions: test other macroeconomic indicators (unemployment, inflation) and explore transfer function models for richer multivariate analysis.
