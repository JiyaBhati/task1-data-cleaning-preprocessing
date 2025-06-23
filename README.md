Data Cleaning and Preprocessing : The goal was to clean and prepare raw data for ML. 
I used Google Colab to write and run my code.


Step1 : Importing the dataset and understanding its datatype, and structure

First, i imported all the libraries required , then imported the Titanic dataset( sourced : Kaggle)  from MyDrive into Google Colab and got a brief understanding of its content and order using .head() , and used .info() to get the datatype of each column . 

Step2 : I found out the percentage of missing values using .isnull().mean()*100 , finding missing values in 'Age' , 'Embarked' and 'Cabin' . I dealt with them using Median for 'Age' , Mode for 'Embarked' and dropped the column 'Cabin' as it had about 77% missing data and including it would not be considered useful.


Step3 : Categorical columns are'Sex' and 'Embarked' , I Use Label Encoding for 'Sex' ; One-hot encode 'Embarked' and convert the boolean values to int (1/0) 

Step4 : Normalize/Standardize the numerical features 
To get all the numerical features on the same scale i standardized them using StandardScaler 

Step5 : Then i visualized the outliers for numerical columns ( included 'Age' and 'Fare') using boxplot and removed those outliers using IQR method

Finally, i used .head() to view the preprocessed dataset 
I also used .isnull().sum() to confirm that all the missing values have been handled that no missing values remained in the dataset, making the data clean and reading for ML.

Dataset I Used : 
Titanic Dataset 

Tools and Libraries I Used : 
Google Colab 
Python 3
Pandas 
Numpy 
Scikit-learn 
Seaborn 
Matplotlib
