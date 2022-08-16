# Forecasting India S&P BSE SENSEX and USA S&P-500 Using ARIMA and Prophet

[![forthebadge made-with-python](https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=black)](https://www.python.org/) 
![Repo-Size](https://img.shields.io/github/repo-size/strikersps/Forecasting-India-and-USA-Benchmark-Indices-Using-ARIMA-and-Prophet?color=%23ff0000&style=for-the-badge)
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/19I3GRRTxayNGI_QF6kzAeBcfp6L8lGA-?usp=sharing)
------------------------------------------------------------------------------------------------------------------------------------------------------------------
[![GitHub contributors](https://img.shields.io/github/contributors/strikersps/Forecasting-BSE-SENSEX-and-S-and-P-500-Using-ARIMA-and-Prophet.svg)](https://github.com/strikersps/Forecasting-India-and-USA-Benchmark-Indices-Using-ARIMA-and-Prophet/graphs/contributors)
[![Issues-Badge](https://img.shields.io/github/issues/strikersps/Forecasting-India-and-USA-Benchmark-Indices-Using-ARIMA-and-Prophet?style=plastic)](https://github.com/strikersps/Forecasting-India-and-USA-Benchmark-Indices-Using-ARIMA-and-Prophet/issues)
[![Stars-Badge](https://img.shields.io/github/stars/strikersps/Forecasting-India-and-USA-Benchmark-Indices-Using-ARIMA-and-Prophet?style=plastic)](https://github.com/strikersps/Forecasting-India-and-USA-Benchmark-Indices-Using-ARIMA-and-Prophet/stargazers)
[![Fork-Badge](https://img.shields.io/github/forks/strikersps/Forecasting-India-and-USA-Benchmark-Indices-Using-ARIMA-and-Prophet?style=plastic)](https://github.com/strikersps/Forecasting-India-and-USA-Benchmark-Indices-Using-ARIMA-and-Prophet/network/members)

![Dalal Street and Wall Street Photo](https://github.com/strikersps/Forecasting-BSE-SENSEX-and-S-and-P-500-Using-ARIMA-and-Prophet/blob/main/Dalal-and-Wall-Street.jpg)

## 1. Introduction  
- The goal of Time Series Analysis and Forecasting is to deal with the class of data science problems where the primary values of interest are a sequence of data points measured over a period of time or recorded over regular intervals of time or which are equally spaced in time and we want to forecast either a single measurement (univariate) or multiple measurements (multi-variate) using the time-series models. 

- This study forecasts the index close values and volatility dynamics of S&P BSE SENSEX of Bombay Stock Exchange (BSE) and S&P-500 of New York Stock Exchange (NYSE).  

- To achieve the objectives, the study uses descriptive statistics, statistical tests including Augmented Dickey-Fuller for checking the stationarity of the underlying time series data before modeling. The developed models forecasts daily close values for the S&P BSE SENSEX and S&P-500 financial time-series data using the ARIMA model and a suite of time series models provided by a Prophet library developed by Facebook especially for forecasting time series data in the Python programming language.

![SARIMAX-Prophet-Daily-Close-Predictions-SENSEX](https://github.com/strikersps/Forecasting-India-and-USA-Benchmark-Indices-Using-ARIMA-and-Prophet/blob/main/SARIMAX-Prophet-SENSEX-Predictions.png)
![SARIMAX-Prophet-Daily-Close-Predictions-S&P-500](https://github.com/strikersps/Forecasting-India-and-USA-Benchmark-Indices-Using-ARIMA-and-Prophet/blob/main/SARIMAX-Prophet-S%26P-500-Predictions.png)

![Summary of SARIMAX and Prophet Model Performance](https://github.com/strikersps/Forecasting-India-and-USA-Benchmark-Indices-Using-ARIMA-and-Prophet/blob/main/Summary-of-Model-Performances.png)

- The project is inspired by the Kaggle Notebook titled [**A Modern Time Series Tutorial by Rohan Rao.**](https://www.kaggle.com/rohanrao/a-modern-time-series-tutorial)

## 2. Datasets
- The financial time series datasets are collected using either the libraries such as `quandl, investpy` or by [Yahoo Finance website](https://finance.yahoo.com/).  

|Sr. No | Dataset Name  | Time Period | Source of Dataset|
|:------:| :-------------: | :-----------: | :------ |
|1 | S&P BSE SENSEX  | 2000-2020 | Refer `sensex_data_2001_2020.csv` file in `./Datasets/` directory|
|2 | S&P-500 | 2000-2020 | Refer `S&P-500-Price-Action-Historical-Prices-Dataset.csv` file in `./Datasets/` directory| 
|3 | India VIX  | 2008-2020 | Refer `india_vix_data_2008_2020.csv` file in `./Datasets/` directory|
|4 | CBOE VIX | 1990-2020 | Refer `cboe_data_1990_2020.csv` file in the `./Datasets/` directory|

- Although the `*.csv` files present in the `./Datasets/` directory consists of the corresponding datasets, those `./Datasets/*.csv` files are exported from pandas dataframes which are created as a result of accessing the data from `quandle`, `yahoo`, and `investpy` websites/libraries using `DataFrame.to_csv()` method. 

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

## 4. Publications Based on the Work
1. [**S. P. Sharma, J. R. and K. Deepa, "Forecasting India S&P BSE SENSEX and USA S&P-500 Benchmark Indices Using SARIMAX and Facebook Prophet Library," 2022 6th International Conference on Intelligent Computing and Control Systems (ICICCS), 2022, pp. 1523-1530, doi: 10.1109/ICICCS53718.2022.9788127.**](https://ieeexplore.ieee.org/document/9788127)

```bibtex
@inproceedings{9788127,
	title        = {Forecasting India S&P BSE SENSEX and USA S&P-500 Benchmark Indices Using SARIMAX and Facebook Prophet Library},
	author       = {Sharma, Suraj Prakash and R., Jeyanthi and Deepa, K.},
	year         = 2022,
	booktitle    = {2022 6th International Conference on Intelligent Computing and Control Systems (ICICCS)},
	volume       = {},
	number       = {},
	pages        = {1523--1530},
	doi          = {10.1109/ICICCS53718.2022.9788127}
}
```
##### NOTE: To cite our work, please add the above block of code into your `*.bib` file in the latex environment and if you want to cite this repository, then please copy the meta-data information from `cite this repository` option as shown in the tutorial: https://github.blog/wp-content/uploads/2021/08/GitHub-citation-demo.gif

###### GNU General Public License v3.0  
[![License-Badge](https://img.shields.io/github/license/strikersps/Forecasting-India-and-USA-Benchmark-Indices-Using-ARIMA-and-Prophet?style=for-the-badge&color=red)](Forecasting-India-and-USA-Benchmark-Indices-Using-ARIMA-and-Prophet/blob/main/LICENSE)
