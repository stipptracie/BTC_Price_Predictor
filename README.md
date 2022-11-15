# BTC Price Predictor

[Planning doc]()

[Google Slides Presentation]()

The goal of this notebook is to 


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

[Pycaret](https://pycaret.org/) - PyCaret is an open-source, low-code machine learning library in Python that automates machine learning workflows.

---

## Installation Guide

First check that all of the anaconda associated packages have been installed by running:

```python
    conda list jupyter
    conda list pandas
```

Next the packages not included need to be installed and this can be accomplished by entering the following in the Git Bash terminal.

```python
    pip install questionary
    pip install python-dotenv
    pip install -U pycoingecko
    pip install twilio
```

To check that all of the dependencies have been installed by entering the following into the Git Bash Terminal:

```python
    conda list questionary
    conda list dotenv
    conda list pycoingecko
    conda list twilio
```

With all of these packages the conda environment should be set up to run the BTC Price Predictor application

---

## Usage



---

## Highlights:

### Data Analysis

First we called the data for each individual cyrptocurrency: below is an example for one symbol.

![ripple](images/ripple_analysis.png)

Next we gathered the pct change and then took the absolute value to reflect the magnitude of the change:

![ripple_mag](images/ripple_pct_change.png)

Then we calculated the mean of pct change over the entire 18 months.  This is the threshold for each coin.

![ripple_threshold](images/ripple_threshold.png)

Finally we put all of the values in a combined dataframe for referencing during our comparisons:

![final](images/final_data_threshold.png)

The final thing we had to do was create a concatenated dataframe with two weeks of the most recent cryptocurrency data for the list given to the user. Then we had to compare each day's price against the threshold that we made. This looks like the following:

![2_week](images/2_week_pct_change.png)

This was a complicated conditional logic feat which was accomplished by looping through the symbols in the list. then looping through each day in the two week percent change data frame indexed on the symbol. Then comparing the two and pulling the symbols date and value into a list of messages to be sent to the user using twilio. This is displayed as the following: 

![conditional](images/conditional_logic.png)


---

## Contributors

Created by ,  and Tracie Stipp while in the UW FinTech Bootcamp
> Contact Info:
>
> email: |
> [GitHub]() |
> [LinkedIn]()
>
> email: stipptracie@gmail.com |
> [GitHub](https://github.com/stipptracie) |
> [LinkedIn](https://www.linkedin.com/in/tracie-stipp-0719691b/)
>
> email:  |
> [GitHub]() |
> [LinkedIn]()

---

