\#S\&P 500 Time-Series Forecasting



A comparative modeling project examining whether time-series methods and additional market information improve the prediction of S\&P 500 closing prices.



\## Project Overview



This project was completed as part of the MATH 350 Research Methods course at Nazarbayev University in a three-person team.



The analysis uses 10 years of S\&P 500 market data, comprising 2,515 daily observations. The project compares regression-based and time-series approaches and examines the effect of incorporating additional market variables into the models.



\*\*My contribution:\*\* I was responsible for the technical component of the project, including model development, statistical testing, model evaluation, and interpretation of the quantitative results.



\## Research Questions



1\. Do time-series models improve predictive performance compared with regression-based models?

2\. Does incorporating additional market information improve prediction compared with using lagged closing prices alone?



\## Methodology



Four model configurations were evaluated:



\- Linear Regression using lagged closing prices

\- ARIMA using the closing-price series

\- Multiple Linear Regression using lagged prices and additional market variables

\- ARIMAX combining temporal dependence with additional market variables



The analysis included:



\- construction of lagged features

\- Augmented Dickey-Fuller (ADF) stationarity testing

\- first-order differencing for the non-stationary price series

\- chronological 80/20 train-test split

\- model comparison using RMSE and MAE



\## Results



| Model | RMSE | MAE |

|---|---:|---:|

| Linear Regression (lag-only) | 57.60 | 39.57 |

| ARIMA (lag-only) | 58.73 | 41.00 |

| Multiple Linear Regression (full features) | 18.99 | 13.36 |

| ARIMAX (full features) | 18.59 | 13.21 |



ARIMAX achieved the lowest prediction error, with an RMSE of 18.59 and MAE of 13.21.



The comparison also showed that incorporating additional market variables produced a substantially larger improvement in predictive performance than changing from a regression-based to a time-series model alone.



\## Tools



\- Python

\- pandas

\- NumPy

\- scikit-learn

\- statsmodels

\- matplotlib



\## Repository Structure



```text

sp500-forecasting/

├── notebooks/

│   └── sp500\_forecasting.ipynb

├── README.md

├── requirements.txt

└── .gitignore

```



\## Author



\*\*Aigerim Yeleussizova\*\*  

B.Sc. Mathematics, Nazarbayev University

