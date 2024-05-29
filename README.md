# ML_Project3_Heart_Failure_Classification


# 1. Introduction:
We developed a classification model to predict outcomes based on features. This model helps determine the likelihood of a positive result given these personal attributes.

# 2. Description of the dataset:

#### 2.1 Shape of our Dataset:
Our dataset has 303 rows and 14 columns

![test1](https://github.com/Mervin50/ML_Project3_Heart_Failure_Classification/assets/167336864/384afdfe-6e57-4cf0-b4a4-29231a51bc69)


#### 2.2 Datatypes of our columns:
The datatypes of our columns : 

![test2](https://github.com/Mervin50/ML_Project3_Heart_Failure_Classification/assets/167336864/0db3b85f-faa1-43f8-bcef-b415e66b5c6b)


# 3. Preprocessing and Data Cleaning for EDA

#### 3.1 Detecting Null values in our dataset:

![test3](https://github.com/Mervin50/ML_Project3_Heart_Failure_Classification/assets/167336864/9a73988e-e26d-4e9b-94db-4253fb3e92b1)

There are 2 each null values in chol and thalachh columns. There is one null value in oldpeak column. 

#### 3.2 Evaluating the best technique for handling null values:

![test1](https://github.com/Mervin50/ML_Project3_Heart_Failure_Classification/assets/167336864/b477e4eb-27a5-4e84-a3ef-cfc98938a7d6)

Plot is left skewed, hence we will use median technique for age column.

![test2](https://github.com/Mervin50/ML_Project3_Heart_Failure_Classification/assets/167336864/64a98d03-26b1-415f-a80e-a03892b6c85f)

Plot is right skewed, hence we will use median technique for Smokes column.

![test3](https://github.com/Mervin50/ML_Project3_Heart_Failure_Classification/assets/167336864/6b7e85f0-c10d-4bf5-b24c-a83d30f24a65)

Plot is slightly left skewed, hence we will use median technique for Alkhol column.

#### 3.3 After Treating Null values:

![test1](https://github.com/Mervin50/ML_Project2_LungCancer_Classification/assets/167336864/21b08ffb-e135-4110-8327-5b1fcae24ba5)

We have replaced our null values with median values in three columns : chol, oldpeak and thalachh.

#### 3.4 Assessing Dataset Balance: 

![test1](https://github.com/Mervin50/ML_Project2_LungCancer_Classification/assets/167336864/7fdb2e12-a8d0-4743-b83f-bc26df76f5dd)

We have ratio of 32-29, so its fairly balanced dataset, so no further action is needed to balance the dataset

# 4. Exploratory Data Analysis

#### 4.1 Overview of dataset using statistics:

![test1](https://github.com/Mervin50/ML_Project3_Heart_Failure_Classification/assets/167336864/4bbeb5ae-a422-4a4d-9ee2-fdfc074ab488)

Observation:

1) Cholesterol levels show significant variability, with values ranging from 126 to 564 mg/dl and a high standard deviation of 51.63 mg/dl, indicating a wide range of cholesterol levels among the subjects.
   
2) Mean age is 54.37 years, indicating a heart failures are mostly caused in middle-aged to elderly population.

#### 4.2 Plotting countplot to know distribution of age column.

![test2](https://github.com/Mervin50/ML_Project3_Heart_Failure_Classification/assets/167336864/e5b83e02-c667-48d8-bccb-f849e828ac0c)

Majority of the people in our dataset are from age groups 20 to 39.

#### 4.3 Barplot to know Number of Cigarettes smoked by different age groups

![test3](https://github.com/Mervin50/ML_Project3_Heart_Failure_Classification/assets/167336864/c9ada5eb-a143-4f07-87a6-f2702c4bd411)


Observation:

1) Cholesterol levels show significant variability, with values ranging from 126 to 564 mg/dl and a high standard deviation of 51.63 mg/dl, indicating a wide range of cholesterol levels among the subjects.
   
2) Mean age is 54.37 years, indicating a heart failures are mostly caused in middle-aged to elderly population.

#### 4.4 Pie chart to illustrate the distribution of daily drink consumption

![test1](https://github.com/Mervin50/ML_Project2_LungCancer_Classification/assets/167336864/26cc1388-f290-4be4-bce4-04407baf40f5)

Approximately 33% people take 2 to 3 drinks per day

#### 4.5 Barplot to know smoking and drinking habits

![test1](https://github.com/Mervin50/ML_Project2_LungCancer_Classification/assets/167336864/0062e1db-4d16-46cf-958f-2ea3fef6cab5)

From our barplot, we come to know that majority of people do both smoking and drinking.

#### 4.6 Histogram to explore the age distribution of individuals affected by lung cancer

![test1](https://github.com/Mervin50/ML_Project2_LungCancer_Classification/assets/167336864/2bc678db-8207-4ee4-aac0-ef8afa29d600)

Majority of people affected by Lung cancer are approximately above age 47.

#### 4.7 Scatter plot to understand relationship between age and smoking habits for the individuals in the dataset

![test1](https://github.com/Mervin50/ML_Project2_LungCancer_Classification/assets/167336864/b637479c-0ede-4527-98ce-6a261c6aa381)

1) There is an outlier in our dataset where a user smokes approximately 35 cigarettes at the age of 27.

2) Our data appears to be scattered.
   
#### 4.8 Boxplot to visually analyze the distribution

![test1](https://github.com/Mervin50/ML_Project2_LungCancer_Classification/assets/167336864/c5a59816-dca0-41ad-bac2-19a089b0c959)

We plotted a box plot to visually analyze the distribution and spread of the 'Age' and 'Smokes' variables in the dataset. We were not able to see any outliers in our plot

#### 4.9 Heatmap

![test1](https://github.com/Mervin50/ML_Project2_LungCancer_Classification/assets/167336864/56bb8c13-49e6-44e7-8969-38cb933a3297)

Heatmap shows us correlation between our numeric columns
