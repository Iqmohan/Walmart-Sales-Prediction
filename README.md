   ## WALMART SALES PREDICTION 
 TIME SERIES ANALYSIS -SARIMA MODEL

### Problem Statement :
 #### A retail store that has multiple outlets across the country are facing issues in managing the inventory - to match the demand with respect to supply. Dataset Information: The walmart.csv contains 6435 rows and 8 columns.

1. You are provided with the weekly sales data for their various outlets. Use statistical analysis, EDA, outlier analysis, and handle the missing values to come up with various insights that can give them a clear perspective on the following:
​
a. If the weekly sales are affected by the unemployment rate, if yes - which stores are suffering the most?

​
b. If the weekly sales show a seasonal trend, when and what could be the reason?

c. Does temperature affect the weekly sales in any manner?

​
d. How is the Consumer Price index affecting the weekly sales of various stores?

​
e. Top performing stores according to the historical data.

​
f. The worst performing store, and how significant is the difference between the highest and lowest performing stores.

​
#### 2. Use predictive modeling techniques to forecast the sales for each store for the next 12 weeks.

Start - Steps Involved

Step 1 - Importing all the required Libraries for Analysis

Step 2 - Importing the walmart Data set through pandas

### Exploratory Data Analysis


step 3 - Extracting the first 20 rows of the Dataset

step 4 - Fetching the unique values from the 'Store' column

step 5 - Fetching the unique values from the 'Holiday_Flag' column

step 6 - Fetching the datatypes information from every columns of the dataset column

step 7 - converting 'object' datatype to 'datetime' datatype

step 8 - finding the null values



step 9 - finding the duplicates values in the data set

### Statistical Analysis

step 10 - getting transposed Statistical summary

step 11 - Analyzing Correlation between the columns

step 12 -  droping all columns to the new columns 'col' to run the for loop for Outlier Analysis

### Outlier Analysis

step 13 - Outlier Analysis for every columns through for loop 

step 14 -  As per the box plot Analysis ,there are outliers present in these columns : Weekly_Sales, Holiday_Flag, Temperature, Unemployment...

### Outlier removal technique

step 15 - Lets find out the quantiles and inter-quantile-range and remove the outliers as it is not required for the analysis...
#So,lets apply the this technique to remove outlier from the above mentioned columns...


step 16 - Running the loop again to check the outliers:
        
        RESULT: -- No oultiers Present after treating it in all the mentioned columns





## Problem Statements : Solutions

#### A. If the weekly sales are affected by the unemployment rate, if yes - which stores are suffering the most?



solution : Visualize the relationship between Unemployment Rate and Weekly Sales
![S](https://github.com/Iqmohan/Data_Science_Machine_Learning_Projects/assets/159016465/f9c972b6-d777-422d-8c85-3d3e6c2bc0a9)
             
             Correlation between Unemployment Rate and Weekly Sales: -0.10617608965795419.
            
#### The store most affected by changes in the unemployment rate is Store 36 Solution : Clearly ,the correlation of columns 'Weekly_Sales' & 'Unemployment' are negative .there is no such dependency between both of them,so 'Unemployment' its not affecting 'Weekly_Sales'


#### b. If the weekly sales show a seasonal trend, when and what could be the reason?


![Screenshot (1962)](https://github.com/Iqmohan/Data_Science_Machine_Learning_Projects/assets/159016465/67804680-a26d-4cff-b014-5147d8d67cc8)

![Screenshot (1963)](https://github.com/Iqmohan/Data_Science_Machine_Learning_Projects/assets/159016465/95fdc7d6-0384-4a88-b7aa-611ab8653765)


![Screenshot (1964)](https://github.com/Iqmohan/Data_Science_Machine_Learning_Projects/assets/159016465/934e8c5c-8a41-454e-b805-8bc012d5607c)

#### Solution: As per the pattern observed ,weekly sales over time shows seasonal patterns as there are no features variation in the columns


#### c. Does temperature affect the weekly sales in any manner?

![Screenshot (1965)](https://github.com/Iqmohan/Data_Science_Machine_Learning_Projects/assets/159016465/65456d80-e543-4ee8-9d93-232723afee1f)


#### Solution :Temperature is not affecting Weekly sales in any way as it is observed from the scatter plot and correlation matrix

D. How is the Consumer Price index affecting the weekly sales of various stores?

![Screenshot (1966)](https://github.com/Iqmohan/Data_Science_Machine_Learning_Projects/assets/159016465/32e05bd5-97b3-4527-b37e-61595229a3e8)

e. Top performing stores according to the historical data

![image](https://github.com/Iqmohan/Data_Science_Machine_Learning_Projects/assets/159016465/9eb2f999-fa0f-434c-9b32-c19ee5427378)



![image](https://github.com/Iqmohan/Data_Science_Machine_Learning_Projects/assets/159016465/c47e4fc2-4e2a-4fc0-bc73-6677c83fb73f)

![image](https://github.com/Iqmohan/Data_Science_Machine_Learning_Projects/assets/159016465/f155bfa1-4445-49d4-8643-00ff1f8ea211)

### Sales Forecasting using SARIMA Model


#### Model Implementation -- Sales Forecast for 12 weeks -- Stores included here are Stores 1,2,3,4,5 (Generating a Forecasts for all 45 stores increases time complexity,hence did it for only 5 stores for evaluation purpose)


![image](https://github.com/Iqmohan/Data_Science_Machine_Learning_Projects/assets/159016465/497fcf70-bcfc-4537-9727-e50312de69bc)
![image](https://github.com/Iqmohan/Data_Science_Machine_Learning_Projects/assets/159016465/0bef0279-92d9-49e3-b990-06ecc844cea0)
![image](https://github.com/Iqmohan/Data_Science_Machine_Learning_Projects/assets/159016465/2b9d1e1b-b338-4ec0-b7fd-e08e9fdb2ee8)
![image](https://github.com/Iqmohan/Data_Science_Machine_Learning_Projects/assets/159016465/508852d1-a2fc-45e3-b43b-bd452aed59e6)
![image](https://github.com/Iqmohan/Data_Science_Machine_Learning_Projects/assets/159016465/7d993b3c-a856-4175-acb0-94ee7500ce94)




## END OF THE PREDICTION


