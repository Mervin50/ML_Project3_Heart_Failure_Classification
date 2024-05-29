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

Majority of the people in our dataset are from age groups 50 to 64.

#### 4.3 Pie chart to know distribution of subjects by heart attack risk level.

![test3](https://github.com/Mervin50/ML_Project3_Heart_Failure_Classification/assets/167336864/c9ada5eb-a143-4f07-87a6-f2702c4bd411)


Observation:

1) 56.5% of the subjects are at low risk of getting a heart attack, while 45.5% are at high risk.

#### 4.4 Plotting barplot to know heart attack risk by gender.

![test1](https://github.com/Mervin50/ML_Project3_Heart_Failure_Classification/assets/167336864/c3641a45-d70d-4017-8480-0659a99d7af0)

Observations:
1) We came to know from the above plot that males are more prone to Heart attack as comapared to females

#### 4.5 Barplot to know smoking and drinking habits

![test2](https://github.com/Mervin50/ML_Project3_Heart_Failure_Classification/assets/167336864/22a70e48-8d12-47a3-b71c-854d9d500c34)

Observations :
1) From our barplot, we come to know that majority of people do both smoking and drinking.

#### 4.6 Countplot to illustrate the distribution of chest pain

![test3](https://github.com/Mervin50/ML_Project3_Heart_Failure_Classification/assets/167336864/81037562-0508-4a6e-a742-089852055478)

Observations : 
1) Majority of the people suffer from type 0 and type 2 kind of chest pain

#### 4.7 Plotting barplot to know smoking and drinking habits

![test4](https://github.com/Mervin50/ML_Project3_Heart_Failure_Classification/assets/167336864/baa6372e-b2b1-41f6-8ebc-6e82157a553b)

Observation: 
1) As people get older, the heart rate goes down as known
   
#### 4.8 4.6 Plotting plot to know distribution of Age among people who had Heart Attack

![test1](https://github.com/Mervin50/ML_Project2_LungCancer_Classification/assets/167336864/c5a59816-dca0-41ad-bac2-19a089b0c959)

Observation : 
1) Upon visual inspection, it appears that females across all age groups tend to experience heart failure at a later stage compared to males.

#### 4.9 Heatmap

![test1](https://github.com/Mervin50/ML_Project2_LungCancer_Classification/assets/167336864/56bb8c13-49e6-44e7-8969-38cb933a3297)

Heatmap shows us correlation between our numeric columns
