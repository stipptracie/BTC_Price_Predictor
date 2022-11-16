# BTC Price Predictor

[Planning doc](https://github.com/stipptracie/BTC_Price_Predictor/blob/main/ProjectOutline.md)

[Google Slides Presentation](https://docs.google.com/presentation/d/1HGoxUIvRFVSQXJkmUEHEMvzjjBAcIP2ZBC31PUGa6yc/edit#slide=id.p)

The goal of this notebook is to better predict Bitcoin prices using technical indicators, sentiment analysis and machine learning.


---

## Required Installs

### Language: Python 3.7.13

### Libraries used:

[Pandas](https://pandas.pydata.org/pandas-docs/stable/index.html) - For the creation and manipulation of Data Frames

[Jupyter Labs](https://jupyter.org/) - An ipython kernel for interactive computing in python

[Numpy](https://numpy.org/) - NumPy is an open source project aiming to enable numerical computing with Python.

[Talib](https://ta-lib.org/) - TA-Lib is widely used by trading software developers requiring to perform technical analysis of financial market data.

[Pandas_datareader](https://pypi.org/project/pandas-datareader/) - Pandas Datareader is a Python package that allows us to create a pandas DataFrame object by using various data sources from the internet. It is popularly used for working with realtime stock price datasets.

[Sklearn](https://scikit-learn.org/stable/index.html) - Scikit-learn: Machine Learning library, Simple and efficient tools for predictive data analysis

[Pycaret](https://pycaret.org/) - PyCaret is an open-source, machine learning library in Python that automates machine learning workflows.

[Matplotlib](https://matplotlib.org/) - Matplotlib is a comprehensive library for creating static, animated, and interactive visualizations in Python. 

[Hvplot](https://hvplot.holoviz.org/) - HvPlot provides a high-level plotting API built on HoloViews that provides a general and consistent API for plotting data.

[XGBoost](https://xgboost.readthedocs.io/en/stable/install.html) - XGBoost provides binary packages for some language bindings. The binary packages support the GPU algorithm (gpu_hist) on machines with NVIDIA GPUs.

---

## Install
```
# create a conda environment
conda create --name yourenvname python=3.8

# activate conda environment
conda activate yourenvname

# install pycaret
pip install pycaret

```
If that doesn't work try:
```
# install the full version of pycaret
pip install pycaret[full]
```

---

## Data
- BTC price data pulled from Yahoo Finance. 
- Technical indicators created using Talib. 
- BTC sentiment indicator pulled from alternative.me using the following:

```
r = requests.get('https://api.alternative.me/fng/?limit=0')
r.json()
df = pd.DataFrame(r.json()['data'])
```

### Data Analysis




---

## Contributors

Created by Ryan Granston, Austin Means and Tracie Stipp while in the UW FinTech Bootcamp
> Contact Info:
>
> email: |
> [GitHub]() |
> [LinkedIn]()
>
> email: |
> [GitHub]() |
> [LinkedIn]()
>
> email: stipptracie@gmail.com |
> [GitHub](https://github.com/stipptracie) |
> [LinkedIn](https://www.linkedin.com/in/tracie-stipp-0719691b/)
>

---

