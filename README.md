# vignette-linearregression-ts
Vignette on Linear Regression with Time Series for PSTAT 197A in Fall 2025

# Contributors
Priyanka Durai, Benjamin Hurt, Alex Dieter, Wendy Zhu
 

# Vignette Abstract
Our vignette focuses on a time-series analysis of products sold at Favorita stores in Ecuador. Using historical sales data, we build a forecasting model to predict sales across product families and stores (Favorita).  

We base our model on seven CSV files provided in the Kaggle "Store Sales - Time Series Forecasting" (https://www.kaggle.com/code/ryanholbrook/linear-regression-with-time-series/data).  

Most notably, the file `train.csv` contains the main training data. Important attributes/columns for this file include:  
- `store_nbr`: store identifier  
- `family`: type of product  
- `sales`: total sales for a product family (fractional values possible)  
- `onpromotion`: number of items promoted at a given date  

Through a time-series approach, we intend to capture shopping behavior patterns (which relate to sales at any given time) and accurately forecast sales for Favorita stores in Ecuador. 

In our practice of applying linear regression to time series data, we construct a simple linear regression model fitted using the Ordinary Least Squares (OLS) method. The response variable — daily average sales — is obtained by loading the original dataset and aggregating each individual sale into a single average value for each date. To build the model, we treat time as the main explanatory factor, and the independent variable is represented by a time index that increases sequentially across the observation period. This setup allows us to capture the overall trend in sales over time and provides a straightforward starting point before incorporating more complex time-series features. 

# Repository Contents
📂 Repository  
├── 📂 data  
│   ├── book_sales.csv      # book sales dataset  
│   └── test.csv            # test dataset from our Kaggle  
│  
├── 📂 scripts  
│   ├── 📂 drafts  
│   │   └── alex.ipynb      # notebook draft  
│   └── vignette-script.py  # main vignette script that sources the Kaggle and builds model  
│  
├── .gitignore              # git ignore stuff  
├── README.md               # what you're reading!  
└── vignette.ipynb          # vignette notebook/report  

(AI-generated diagram for brevity's sake, since trying to use arrows made it convoluted)

- In words, the repository contains a folder with our data taken from the Kaggle dataset. There also exists another folder that contains our scripts for processing the data and building the model. 

# Reference List
- According to guidelines, 'Reference list: 2 or more references to learn more about your topic.'
- https://www.kaggle.com/code/ryanholbrook/linear-regression-with-time-series/data
