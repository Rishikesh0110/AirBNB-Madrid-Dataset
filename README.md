#Table of contents
1. Introduction
2. Description of the data set
3. Intorduction about the python libraries.
4. Initial steps
5. Info of data
6. Descriptive statistics
7. Start looking at Numerical columns of data
8. Start lookin at categorical columns of the data
9. Looking at after combining both numerical and categorical columns
10. Data wrangling
11. Handling missing values
12. Handling duplicates
13. Handling outliers
14. Handlig numerical and categorical columns

# Madrid-AirBnb-Analaysis

This is exploratory data analysis about the Madrid listings in AirBnb, The main purpose of this project to draw insights from AirBnb spain dataset.
To know further about AirBnB phenomenon in Madrid as it is very populer accomoation business across the city, The more information about the data can help peoples to take better decisions about AirBnB on facts.
# About the data
DataSetInformation: https://www.kaggle.com/datasets/rusiano/madrid-airbnb-data?select=listings.csv
This data file includes all needed information to find out more about hosts, geographical availability, necessary metrics to make predictions and draw conclusions.
Details of fields. https://docs.google.com/spreadsheets/d/1iWCNJcSutYqpULSQHlNyGInUvHg2BoUGoNRIGa6Szc4/ edit#gid=1322284596



## Installation & Tools

For withdraw insights from the data ,we must have the following python liberies installed to
analyse data deeply.

**numpy**
NumPy (Numerical Python) is an open source Python library that’s used in almost every field of science and engineering. It’s the universal standard for working with numerical data in Python.
https://numpy.org/doc/stable/user/absolute_beginners.html

**Pandas**
pandas is an open source, BSD-licensed library providing high-performance, easy-to-use data structures and data analysis tools for the Python programming language.
https://pandas.pydata.org/docs/

**Seaborn**
Seaborn is a Python data visualization library based on matplotlib. It provides a high-level interface for drawing attractive and informative statistical graphics.
https://seaborn.pydata.org/

**Matplotlib**
Matplotlib is a comprehensive library for creating static, animated, and interactive visualizations in Python.
https://matplotlib.org/

**Sklearn**
Simple and efficient tools for predictive data analysis
https://scikit-learn.org/stable/

## Questions which need to be answere 
1. Which room type has served at what average cost?
2. Which type of rooms are used most by people?
3. Average price near each neighbouhood?
4. Which of the neighbourhood group are most famous across the Madrid?
5. Which room type has highest no. of reviews?
6. Which type of room got highest number of reviews per month?
7. Any relation b/w reviews and use of the rooms?
## Introduction and Methods
1.**Loading the data**
1. Loaded each liabraried first like numpy,pandas,matplotlib,seaborn
1. This data describes  the Madrid AirBnB data we can check for each columns by head() & tail functions.
The analysis takes the form of a single Google colab notebook of filename given above. 

I have tried to structure the Google colab notebook and this README so anyone can easily understood the project. 

2. After loading the libraried i read the dataset with help of pandas. pd.read_csv("path_name").
3. **Description of dataset**  This data file includes all needed information to find out more about hosts, geographical availability, necessary metrics to make predictions and draw conclusions.
Details of fields. https://docs.google.com/spreadsheets/d/1iWCNJcSutYqpULSQHlNyGInUvHg2BoUGoNRIGa6Szc4/ edit#gid=1322284596
4. **Initial steps** After uploaded and read the data in notebook ,i have look on the data first five rows and last five rows by head() and tail(). Afetr checking head and tail of data i checked shape of data and information of data by .shape & .info().
5. **Descriptive statistics** Pandas describe() can provide a quick summary of the data set as outlined in the notebook. And .describe(include="O") to check categorial description.
From above summary we can say that:
We have the airbnb dataset for anaysis in which we have details about Airbnb listings in Madrid, Spain..
This data set have total number of columns 16 numerical & categorical both.
Airbnb dataset have total number of rows 19,618.
**Exploratory data anlysis**
   1. looked over each and every column to get the overall view of the data and extract insights by:
7. **Looking at categorical and numerical columns**
Now exloratory data analysis started , i draw distribution plot, box plot, Histogram plot for each numerical columns by help of seaborn and matplotlib, and also finded mean value, skewness, variance , standard daviation for each numerical columns in the dataset.
8. We get for each categorical clumns there total number unique values by **nunique()** and check the values by **unique()** and counted the values by **Value_counts()** after than i draw countplot and pie plots to visualize the insights.
9. **GroupBy** Applied groupby and diffrent techniques to combine the coulumns of data to draw insights and visualie by barplots and catplots.
10. After done all analysis i checked correlation b/w all the coluns to check any other factor affecting other facors or not by corr().
11. Than i used datawrangling such as handled missing values with help of **Drop_duplicates()** and checked shape of data wether duplicates available or not, than i Used **Isnull()**to find nan values and if there is any missing values have than filled wih mean value of the specific columns.
12. **Data wranggling**
13. Founded missing values by help of df.isnull().sum() , and handled with the respective median and mean of the columns.
14. Than handled duplicates which available in data by help of drp_duplicates.
15. Handled outlier by find quantiles at 25% of data 50% of data and 75 % of data, with the help of formula IQR(inter quartile range)= 75%-25% portion of data. than founded minimum whisker and maximum whisker and handled outliers by median of the columns,
16. **Standarizations of each columns**
17.  Handled categorical columns by
18. **One hot encoding** pd.get_dummies() and numerical columns by minmax scaler and stadard scaler to standarize numerical columns.
19. **Scaler** MinMax and Standard scaler used to heandle the numerical columns of the data.
20. ## Conclusions
21. So by this analysis i founded every importand answers such as which room type are most chepest and costly ,which neibhourhood are most famous that are some more insights which can help this business to learn a business pattern they serve.
22. ## Acknowledgements
I want to thank Topmentor teams & my mentor Mr. Ved  sir to make me able to use these tools which helps to drive insights from the data and also thankfull for team to provided such AirBNB data otherwise the project could not have been done.
