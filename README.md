## **Yalini Brhanavan - GMIT - H.Dip Data Analytics**

<img src="https://image.ibb.co/gw4Gen/Index_GMIT.png" alt="Index GMIT" border="0" />

* Fundamentals of Data Analysis: Project 2020
* Sep 2020

---

**How to run the file:**
1. Open Task 2020.ipynb in Jupyterlab or Jupyter notebook .
2. Import following libraries pandas, numpy and matplotlib.pyplot
3. Click the Kernel button and select Restart & Run All. 
4. when the pop window appear select Restart and Run All Cells. 
-----

**Project Instructions:**

This project has the following sections :

1.  <span style="color:blue"> *Read data from the flat file powerproduction.txt*</span> <br/>
Read Power production data file using Pandas </br>
<code>  df_power = pd.read_csv('powerproduction.txt') </code> <br/>

2. <span style="color:blue"> *Performs a simple linear regression to analyse the relationship between Wind Speed and Power Production*</span> <br/> 
Simple linear regression are of the form y = m x + c
I have compared Simple Linear Regression Using Numpy Plotfit vs Using Scikit Learn. 
* Simple Linear Regression Using Numpy Plotfit<br/> 

<img src="Linear model Numpy Poltfit.png" alt="Linear model Numpy Poltfit plot" width="50%"><br/> 
*  Simple Linear Regression Using Scikit Learn
<br/> 
<img src="Linear Model Scikit Learn.png" alt="Linear Model Scikit Learn plot" width="50%"><br/> 
Both of these models essentially produced the same linear relationship. 
<br/> 
* Linear Model : Predicted vs Actual Values
<img src="Linear Model_predicted vs Actual values.png" alt="Linear Model Scikit Learn plot" width="50%"><br/>
The scatterplot of predicted power values and actual values shows the model is good fit between when power values are between 20 and 80. This is because the linear relationship speed and power breaksdown when the speed is less than 10 or speed is over 20. <br/>

Because the linear model is not a great fit , next I tried to fitting a higher order polynomial. <br/>
3. <span style="color:blue"> *Explores other regression model to see if the predictive power could be improved*</span> <br/> 
 Fit a third degree polynomial using Numpy Plotfit
<br/> 
<img src="3rd Degree polynomial_Predicted vs Actual Values.png" alt="Third Degree polynomial : Predicted vs Actual Values" width="50%"><br/>

This relationship appears to be a better fit than the linear model. However the 3rd degree plotfit predictions are not accurate when the wind speed is greater than 20. 


----
**REFERENCES:** 
1. Read Data: 
* [Pandas- read_csv documentation](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.read_csv.html)
* [Geek for geeks - using pandas.read_csv](https://www.geeksforgeeks.org/python-read-csv-using-pandas-read_csv/)

 2. Simple Linear Regression Using Numpy Plotfit : 
* [Pandas to_numpy() method](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.values.html)
* [FDA Lectures-Topic 9 Fitting Lines](https://github.com/ianmcloughlin/jupyter-teaching-notebooks/blob/master/fitting-lines.ipynb)
* [FDA Lecture-Topic 9 Simple Linear Regression](https://github.com/ianmcloughlin/jupyter-teaching-notebooks/blob/master/simple-linear-regression.ipynb)
3. Simple Linear Regression Using Scikit Learn 
* [Scikit Learn Linear Regression Documentation](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LinearRegression.html)
* [Datacamp - Essentials of Linear Regression in Python](https://www.datacamp.com/community/tutorials/essentials-linear-regression-python)