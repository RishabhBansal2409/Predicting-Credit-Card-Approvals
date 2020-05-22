Built a **supervised Machine Learning classifier** which predicts **whether a Credit Card application will get approved or not** taking into account the below features :
* Gender 
* Age   
* Debt  
* Married   
* BankCustom: 
* EducationLevel  
* Ethinicity
* YearsEmployed 
* PriorDefault  
* Employed   
* CreditScore Citizen   
* Income  
* ApprovalStatus  

Data is sourced from the [UCL repostory](http://archive.ics.uci.edu/ml/datasets/credit+approval).

Below are the set of steps executed in order to build the Credit Card application approval prediction model. 

1. **Importing Libraries and loading data**.

2. **Exploratory data Analysis (EDA)** to know the issues in the dataset beforehand.Issue observed are as follows:
    * Dataset contains **numeric and non-numeric columns**.
    * Datasets' **numeric features have different ranges**.
    * **Detection of missing values** which are labeled as ?.
    
3. **Handling of the missing values** by following the below approaches.
    * Replace the missing values **labeled with ? with NaN**.
    * **Mean Imputation** for the numerical variables
    * Impute missing values in **non-numeric columns** with the **most frequent values** as present in the respective columns.

4. Converting the **Non-Numeric data into Numeric using Label Encoder**.
   
5. Check if **the data is balanced or imbalanced** by comparing the no of approved and not approved applications.

6. Dropping the **columns such as DriversLicense and ZipCode** based on domain knowledge.This is known as **Feature Selection**.

7. **Splitting** the data into **training and testing set** for two different phases of machine learning modeling: training and testing.

8. **Scaling the data to the range of 0-1**.

9. **Fitting a logistic Regression** to the training set.

10. **Making predictions** and **evaluating performance**.

11. **Grid searching** and making the model perform better.

12. **Finding the best performing model**.
