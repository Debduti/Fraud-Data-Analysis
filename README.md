# Fraud-Data-Analysis
In this project we use a publicly available dataset ,clean and analyse all its features to understand which features might be the biggest factors to determine whether a transaction is Fraud.
Credit Card Frauds are one of the biggest reasons for chargebacks and disputes raised against a merchant. The onus is often on the merchant and the aquirer bank to resolve the dispute and refund any money the cardholder ows due to incorrect posting of transaction on their credit card statement. 
Here is where a robust Fraud Detection System plays a crucial role. It would save the financial institutions billions of dollars if they can have such checks and balances in place so that before they process their transaction for the day, they can segregate the Fraud transactionsn and take action as necessary.

# Aim of this project
This project has 4 main objectives
a. To clean the data that has been extracted/sourced. This involves inspecting the null values and deciding to either 
  i. Replace them with default values like 0 
  ii. Remove the row or the column altogether. Not a recommended method if there are not many rows or features to begin with, as it impacts the quality of data and might remove a    key feature
  iii. Impute them with a value that is a best fit in the scenario. So it could be either the mean of all the remaining values if the distribution is fairly uniform, or the median for a more d=skewed distribution etc.
  
 # Methodology
 We use Python language to accomplish this project.
 The various libraries that we have used are
 a. Pandas
 b. Numpy
 c. Sci-Py
 d. Matplotlib
 e. Seaborn
 ## Steps
 1. The dataset(source: Kaggle) is in a CSV format. It is then read into a Pandas Dataframe. We do some basic analysis of the dataset to find out what it looks like, its size,datatypes, record counts,column counts.
 2. We then move on to check for Null/Missing values in any of the columns and rows. The dataset is fairly clean , so no handling of missing values was required.
 3. We then check for duplicate transactions and remove all duplicates, so that the resultant file has unique transactions only. 
 4. We nominate 'Class' as the target variable. It can have a value of either 0, meaning genuine transaction or 1, meaning Fraud transaction. For any subsequent machine learning model, the aim would be to predict the value of Class given a set of the other parameters.
 5. We check the distribution of the all the parameters to get a fair idea about the range of their values.
 6. We create and plot a correlation matrix to help us choose the best probable features to create our models.
 # Scope
 The scope of this project is to do an Exploratory Data Analysis of the Fraud Dataset. In subsequent versions of this project we will build some machine learning models to predict whether a transaction is Fraud or not.
