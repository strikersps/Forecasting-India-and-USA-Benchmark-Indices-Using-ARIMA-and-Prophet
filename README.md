# Forecasting India S&P BSE SENSEX and USA S&P-500 Using ARIMA and Prophet

[![forthebadge made-with-python](https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=black)](https://www.python.org/) 
![Repo-Size](https://img.shields.io/github/repo-size/strikersps/Forecasting-India-and-USA-Benchmark-Indices-Using-ARIMA-and-Prophet?color=%23ff0000&style=for-the-badge)
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/19I3GRRTxayNGI_QF6kzAeBcfp6L8lGA-?usp=sharing)
------------------------------------------------------------------------------------------------------------------------------------------------------------------
[![GitHub contributors](https://img.shields.io/github/contributors/strikersps/Forecasting-BSE-SENSEX-and-S-and-P-500-Using-ARIMA-and-Prophet.svg)](https://github.com/strikersps/Forecasting-BSE-SENSEX-and-S-and-P-500-Using-ARIMA-and-Prophet/graphs/contributors)
[![Issues-Badge](https://img.shields.io/github/issues/strikersps/Forecasting-BSE-SENSEX-and-S-and-P-500-Using-ARIMA-and-Prophet?style=plastic)](https://github.com/strikersps/Forecasting-BSE-SENSEX-and-S-and-P-500-Using-ARIMA-and-Prophet/issues)
[![Stars-Badge](https://img.shields.io/github/stars/strikersps/Forecasting-BSE-SENSEX-and-S-and-P-500-Using-ARIMA-and-Prophet?style=plastic)](https://github.com/strikersps/Forecasting-BSE-SENSEX-and-S-and-P-500-Using-ARIMA-and-Prophet/stargazers)
[![Fork-Badge](https://img.shields.io/github/forks/strikersps/Forecasting-BSE-SENSEX-and-S-and-P-500-Using-ARIMA-and-Prophet?style=plastic)](https://github.com/strikersps/Forecasting-India-and-USA-Benchmark-Indices-Using-ARIMA-and-Prophet/network/members)

![Dalal Street and Wall Street Photo](https://github.com/strikersps/Forecasting-BSE-SENSEX-and-S-and-P-500-Using-ARIMA-and-Prophet/blob/main/Dalal-and-Wall-Street.jpg)

## 1. Introduction  
- The goal of Time Series Analysis and Forecasting is to deal with the class of data science problems where the primary values of interest are a sequence of data points measured over a period of time or recorded over a regular intervals of time or which are equally spaced in time and we want to forecast either a single measurement (univariate) or multiple measurements (multi-variate) using the timeseries models. 

- This study forecasts the index close values and volatility dynamics of S&P BSE SENSEX of Bombay Stock Exchange (BSE) and S&P-500 of New York Stock Exchange (NYSE).  

- To achieve the objectives, the study uses descriptive statistics, statistical tests including Augmented Dickey-Fuller for checking the stationarity of the underlying time series data before modeling. The analysis forecasts daily index values for the S&P BSE SENSEX and S&P-500 financial time-series data using the ARIMA model and a suite of time series models provided by a Prophet library developed by Facebook especially for forecasting time series data in Python programming language.  

- `SARIMAX (2, 0, 0) × (2, 0, 0, 7)` for India S&P BSE SENSEX and `SARIMAX (5, 1, 1) × (2, 0, 1, 7)` for USA S&P-500 have given realiable results with a Mean-Absolute-Percentage-Error (MAPE) of `4.05%` and `0.61%` respectively. 

- Prophet based models has performed better than both the ARIMA models when forecasting S&P BSE SENSEX and S&P-500 with MAPE of `1.06%` and `0.62%` respectively.

- The project is inspired by the Kaggle Notebook titled [**A Modern Time Series Tutorial by Rohan Rao.**](https://www.kaggle.com/rohanrao/a-modern-time-series-tutorial)

## 2. Datasets
- The financial time series datasets are collected using either the libraries such as `quandl, investpy` or by [Yahoo Finance website](https://finance.yahoo.com/).  

|Sr. No | Dataset Name  | Time Period | Source |
|:------:| :-------------: | :-----------: | :------ |
|1 | S&P BSE SENSEX  | 2000-2020 | `quandl` library  |
|2 | India VIX  | 2008-2020 | `investpy` library  |
|3 | S&P-500 | 2000-2020 | [Yahoo Finance Website: S&P-500 Price Dataset](https://finance.yahoo.com/quote/%5EGSPC/history?p=%5EGSPC&guccounter=1) or Refer `S&P-500-Price-Action-Historical-Prices-Dataset.csv` file in Datasets folder.| 
|4 | CBOE VIX | 1990-2020 | `investpy` library |

- `investpy` is a really good library which most people don't know about and it provides financial time series data for almost all the indexed financial products/assets which belong to different asset classes which are covered by [https://www.investing.com/](https://www.investing.com/) website. 

## 3. How to Execute  
   - **3.1 Dependencies**  
    The project has dependencies on the following libraries so make sure you have installed those libraries using `pip` package manager using command `python3 -m pip install -r requirements.txt`.  
    1. `quandl`  
    2. `investpy`  
    3. `yfinance`  
    4. `pmdarima`  
    5. `fbprophet`  
    If you get any error regarding `auto_arima()` method of `pmdadrima.arima` submodule then first uninstall the older version of `statsmodels` library and current installation of `pmdarima` and then again install `pmdarima`, no need to install `statsmodels` library as `pmdarima` has a dependency on `statsmodels` which gets automatically installed during the `pmdarima` installation process.

- **3.2 Execution Steps**  
   - To execute the jupyter notebook click on [![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/19I3GRRTxayNGI_QF6kzAeBcfp6L8lGA-?usp=sharing) badge/shield and do remember that the runtime is around **3 Hrs** if you want to run all the cells again.

  - If you have some problems while executing the Google Colab notebook then consider executing it directly through the following Google Drive link.  
**Google Drive Link:** [**Forecasting S&P BSE SENSEX and S&P-500 Using ARIMA and Prophet.**](https://drive.google.com/drive/folders/17RuDveL9qG37_gbPA2vmt_7HgxCipuMA?usp=sharing)  

**NOTE:** **For project explaination, refer the [presentation](https://drive.google.com/file/d/1wo6zmQd_fzlPBcW3QkmqXxgmvAEN0z9g/view?usp=sharing).**

## 4. License
[![License-Badge](https://img.shields.io/github/license/strikersps/Forecasting-India-and-USA-Benchmark-Indices-Using-ARIMA-and-Prophet?color=red&style=for-the-badge)](https://github.com/strikersps/Forecasting-BSE-SENSEX-and-S-and-P-500-Using-ARIMA-and-Prophet/blob/main/LICENSE)
