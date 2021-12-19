![Apache License](https://img.shields.io/hexpm/l/apa)  ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)  [![Made withJupyter](https://img.shields.io/badge/Made%20with-Jupyter-orange?style=for-the-badge&logo=Jupyter)](https://jupyter.org/try)    ![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)   ![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)  ![Made with matplotlib](https://user-images.githubusercontent.com/86251750/132984208-76ce70c7-816d-4f72-9c9f-90073a70310f.png)  ![seaborn](https://user-images.githubusercontent.com/86251750/132984253-32c04192-989f-4ebd-8c46-8ad1a194a492.png)  ![Spyder](https://img.shields.io/badge/Spyder-838485?style=for-the-badge&logo=spyder%20ide&logoColor=maroon)  ![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white) ![udemy](https://img.shields.io/badge/Udemy-EC5252?style=for-the-badge&logo=Udemy&logoColor=white)

![image](https://user-images.githubusercontent.com/86251750/146649330-d0f19936-0049-4aa5-9b18-c28adc9044b6.png)


## Sales Department

* For companies to become competitive and skyrocket their growth, they need to leverage AI/ML to develop predictive models to forecast sales in the future.

* Predictive models attempt at forecasting future sales based on historical data while taking into account seasonality effects, demand, holidays, promotions, and competition.

## Acknowledgements

 - [python for ML and Data science, udemy](https://www.udemy.com/course/python-for-machine-learning-data-science-masterclass)
 - [ML A-Z, udemy](https://www.udemy.com/course/machinelearning/)
 
## Appendix

* [Aim](#aim)
* [Dataset used](#data)
* [Run Locally](#run)
* [Exploring the Data](#viz)
   - [Dashboard](#dashboard)
   - [Matplotlib](#matplotlib)
   - [Seaborn](#seaborn)
* [solving the task](#fe)
* [prediction](#models)

## AIM:<a name="aim"></a>

The objective is to predict future daily sales based on the features. 

## Dataset Used:<a name="data"></a>

we have data from 1115 stores.

    Id: transaction ID (combination of Store and date)
    
    Store: unique store Id
    
    Sales: sales/day, this is the target variable 
    
    Customers: number of customers on a given day
    
    Open: Boolean to say whether a store is open or closed (0 = closed, 1 = open)
    
    Promo: describes if store is running a promo on   that day or not
    
    StateHoliday: indicate which state holiday (a = public holiday, b = Easter holiday, c = Christmas, 0 = None)
    
    SchoolHoliday: indicates if the (Store, Date) was affected by the closure of public schools
    
    StoreType: categorical variable to indicate type of store (a, b, c, d)
    
    Assortment:  a = basic, b = extra, c = extended
    
    CompetitionDistance (meters): distance to closest competitor store
    
    CompetitionOpenSince [Month/Year]:  date when competition was open
    
    Promo2: Promo2 is a continuing and consecutive promotion for some stores (0 = store is not participating, 1 = store is participating)
    
    Promo2Since [Year/Week]: date when store started participating in Promo2
    
    PromoInterval: describes the consecutive intervals Promo2 is started, naming the months
    
    promotion is started anew. E.g. "Feb,May,Aug,Nov" means each round starts in February, May, August, November of any given year for that store
    
    
dataset can be found at [link](https://github.com/pradeepsuyal/Sales_Department/tree/main/dataset)

## Run locally:<a name="run"></a>

Clone the project

```bash
https://github.com/pradeepsuyal/Sales_Department.git
```

Go to the project directory

```bash
  cd Sales_Department
```

Install dependencies

```bash
  npm install
```

Start the server

```bash
  npm run start
```

If you output `pip freeze` to a file with redirect >, you can use that file to install packages of the same version as the original environment in another environment.

First, output requirements.txt to a file.

```bash
  $ pip freeze > requirements.txt
```

Copy or move this `requirements.txt` to another environment and install with it.

```bash
  $ pip install -r requirements.txt
```

## Exploring the Data:<a name="viz"></a>

I have used pandas, matplotlib and seaborn visualization skills.

**Dashboard:**<a name="dashboard"></a>
---------

![SALES DEPT  DASHBOARD](https://user-images.githubusercontent.com/86251750/146665681-7a6b3832-8829-431a-bdd8-7bcd195c2b61.png)


you can see the dashboard at [tableau](https://public.tableau.com/app/profile/pradeep7347/viz/SALESDEPARTMENTDASHBOARD/SALESDEPT_DASHBOARD)


**Matplotlib:**<a name="matplotlib"></a>
--------
Matplotlib is a Python 2D plotting library which produces publication quality figures in a variety of hardcopy formats and interactive environments across platforms. Matplotlib can be used in Python scripts, the Python and IPython shells, the Jupyter notebook, web application servers, and four graphical user interface toolkits.You can draw up all sorts of charts(such as Bar Graph, Pie Chart, Box Plot, Histogram. Subplots ,Scatter Plot and many more) and visualization using matplotlib.

Environment Setup==
If you have Python and Anaconda installed on your computer, you can use any of the methods below to install matplotlib:

    pip: pip install matplotlib

    anaconda: conda install matplotlib
    
    import matplotlib.pyplot as plt

![matplotlib](https://eli.thegreenplace.net/images/2016/animline.gif)

for more information you can refer to [matplotlib](https://matplotlib.org/) official site

**Seaborn:**<a name="seaborn"></a>
------
Seaborn is built on top of Python’s core visualization library Matplotlib. Seaborn comes with some very important features that make it easy to use. Some of these features are:

**Visualizing univariate and bivariate data.**

**Fitting and visualizing linear regression models.**

**Plotting statistical time series data.**

**Seaborn works well with NumPy and Pandas data structures**

**Built-in themes for styling Matplotlib graphics**

**The knowledge of Matplotlib is recommended to tweak Seaborn’s default plots.**

Environment Setup==
If you have Python and Anaconda installed on your computer, you can use any of the methods below to install seaborn:

    pip: pip install seaborn

    anaconda: conda install seaborn
    
    import seaborn as sns
    
![seaborn](https://i.stack.imgur.com/uzyHd.gif)

for more information you can refer to [seaborn](https://seaborn.pydata.org/) official site.

**Screenshots from notebook**

![download](https://user-images.githubusercontent.com/86251750/146649524-3ba9a675-f64d-4be3-9195-8eb86c811eda.png)

![download](https://user-images.githubusercontent.com/86251750/146649530-d8e532cd-13f6-4d4c-9c0d-d4bfeeb5c683.png)

![download](https://user-images.githubusercontent.com/86251750/146649540-c6bc7248-e235-4d61-8a35-aba950607f06.png)

![download](https://user-images.githubusercontent.com/86251750/146649549-df93d68f-fe1e-4d16-8756-971be998686f.png)


## approach for making prediction<a name="fe"></a>
-------

* first I explored the dataset through visualization to gain the insights 
* Handled missing values
* separated the year,day and month from Date column and put it into a separate column so that I can see the sales a/t year, day and month
* Trained the model with FACEBOOK PROPHET

## Prediction:<a name="models"></a>
------

**FACEBOOK PROPHET**

* Prophet is open source software released by Facebook’s Core Data Science team.
* Prophet is a procedure for forecasting time series data based on an additive model where non-linear trends are fit with yearly, weekly, and daily seasonality, plus holiday effects. 
* Prophet works best with time series that have strong seasonal effects and several seasons of historical data. 
* For more information, please check this out: 
   https://research.fb.com/prophet-forecasting-at-scale/
   https://facebook.github.io/prophet/docs/quick_start.html#python-api
* Prophet implements an additive regression model with four elements:
      
      A piecewise linear, Prophet automatically picks up change points in the data and identifies any change in trends.  
      A yearly seasonal component modeled using Fourier series.
      A weekly seasonal component.
      A holiday list that can be manually provided.
* Additive Regression model takes the form: 

![4](https://user-images.githubusercontent.com/86251750/146649959-b6275214-3e6d-4317-a99a-bb3ad399a48c.PNG)
The functions 𝒇_𝒋 (𝒙_𝒋) are unknown smoothing functions fit from the data 

[reference](https://research.fb.com/prophet-forecasting-at-scale/)

![image](https://user-images.githubusercontent.com/86251750/146650066-13de016d-61e4-4536-a209-53204e4d5fff.png)

![download](https://user-images.githubusercontent.com/86251750/146650106-56a328a2-181b-4d49-b40a-61b29f0aa00b.png)
![download](https://user-images.githubusercontent.com/86251750/146650113-5b39eebe-53a4-441e-8285-c3ea69414b92.png)
