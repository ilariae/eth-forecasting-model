# Ethereum Forecasting Model

A university data analysis and time-series forecasting project focused on understanding and predicting Ethereum price behavior using historical market data.

This project combines exploratory data analysis, statistical interpretation, feature inspection, regression-based reasoning, and forecasting techniques to study Ethereum price dynamics. The main forecasting target is the **daily high price of ETH**, using both **ARIMA** and **Prophet** as comparative forecasting approaches.

## Project overview

Ethereum is a decentralized, open-source blockchain platform with smart contract functionality. Ether (ETH) is its native cryptocurrency and one of the most widely traded digital assets.

The goal of this project is not to build a production trading system, but to explore how historical Ethereum price data can be analyzed, transformed, and modeled in an academic forecasting setting.

## Dataset

The dataset contains the history of daily Ethereum prices from **09-Aug-2015** to **07-Jul-2021**.

Source:  
<https://www.kaggle.com/datasets/sudalairajkumar/cryptocurrencypricehistory>

The analysis uses historical price-related features such as:
- open price,
- close price,
- high price,
- low price,
- volume,
- market capitalization,
- date/time information.

## Main objectives

This project was designed to:
- explore and summarize the Ethereum dataset,
- understand the statistical behavior of the main variables,
- visualize distributions and price trends,
- inspect feature relationships,
- study how variables influence the forecasting target,
- apply transformations where useful,
- fit time-series forecasting models,
- compare different forecasting approaches.

## What the project includes

### 1. Data exploration
The notebook begins with exploratory analysis of the Ethereum dataset, including:
- mean, median, and mode,
- summary statistics,
- outlier inspection,
- feature distributions,
- data types,
- feature explanations,
- visual exploration of the variables.

### 2. Data visualization
The project uses visual analysis to better understand the behavior of Ethereum prices and related variables. This helps identify trends, skewness, variation, and possible modeling issues before forecasting.

### 3. Feature understanding and regression reasoning
A stepwise regression phase is used to better understand how different variables influence the model in a broader statistical sense. This helps interpret the data holistically rather than treating forecasting as a pure black-box exercise.

### 4. Forecasting target
The main target of the project is the **forecasting of Ethereum high prices**.

### 5. Transformation
The project includes a **Box-Cox transformation** to improve modeling assumptions and better handle non-normality or variance instability in the data.

### 6. Model fitting
The project applies **ARIMA** as a classical time-series modeling approach.

### 7. Forecasting comparison
The project also uses **Prophet** as a second forecasting approach in order to compare results and modeling behavior.

## Methodology

The workflow follows a typical forecasting pipeline:

1. load and inspect the Ethereum dataset,
2. clean and understand the available variables,
3. normalize and visualize relevant features,
4. study distributions and descriptive statistics,
5. explore relationships between variables,
6. apply transformations where helpful,
7. fit forecasting models,
8. compare forecasting approaches,
9. interpret the results.

## Tools and libraries

This project is implemented as an **R notebook** (`.ipynb` format) rather than a Python notebook.

The notebook uses a range of R libraries for:
- data cleaning,
- visualization,
- regression,
- time-series analysis,
- forecasting.

These include packages such as:
- `tidyverse`
- `ggplot2`
- `dplyr`
- `lubridate`
- `caret`
- `car`
- `leaps`
- `fpp2`
- `astsa`
- `plotly`
- `timetk`
- `prophet`

## Repository structure

```text
eth-forecasting-model/
├── README.md
├── .gitignore
└── eth-prediction-dv-project.ipynb
```

## Notes on reproducibility

This repository is best understood as an academic notebook project rather than a packaged forecasting application.

A few practical notes:
- the notebook is written in **R**, even though it is stored as a Jupyter notebook,
- the dataset is expected from the Kaggle source referenced above,
- recreating the full environment may require manually installing the R libraries used in the notebook,
- notebook outputs may be large depending on saved visualizations and rendered results.

## Limitations

- Cryptocurrency markets are highly volatile and noisy.
- Historical forecasting performance does not imply trading usefulness in real market conditions.
- The project is intended as an academic forecasting exercise, not as a production-grade financial model.
- Model assumptions may break under strong regime changes or sudden market events.
- The repository focuses on the notebook analysis rather than on packaging, deployment, or automated reproducibility.

## Summary

This project showcases an academic workflow for exploring Ethereum price data and comparing classical and modern forecasting approaches. It combines descriptive analysis, transformation, regression-based reasoning, and time-series forecasting to study the behavior of ETH prices in a structured way.
