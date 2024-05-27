# ML_Project3_Heart_Failure_Classification

# Table of contents

#### 1. Introduction

#### 2. Description of the dataset

     2.1 Head of our Dataset
    
     2.2 Tail of our Dataset

#### 3. Preprocessing and Data Cleaning for EDA

     3.1 Detecting Null values in our dataset

     3.2 Evaluating the best technique for handling null values

     3.3 After Treating Null values

     3.4 Assessing Dataset Balance

     3.5 Label Encoder

  #### 4. Exploratory Data Analysis

     4.1 Overview of dataset using statistics

     4.2 Barplot to know distribution of age column

     4.3 Barplot to know Number of Cigarettes smoked by different age groups

     4.4 Pie chart to illustrate the distribution of daily drink consumption

     4.5 Barplot to know smoking and drinking habits

     4.6 Histogram to explore the age distribution of individuals affected by lung cancer

     4.7 Scatter plot to understand relationship between age and smoking habits for the individuals in the dataset

     4.8 Boxplot to visually analyze the distribution

     4.9 Heatmap

  #### 5. Polishing our dataset for model training

     5.1 Outlier detection and treating using Z-score

     5.2 One-Hot Encoding 

     5.3 Standarization

  #### 6. Model Building and Model Evaluation
     
     6.1 Calculating accuracy of our models

     6.2 Calculating Precision, R2 score and F1 score

     6.3 Calculating confusion Matrix

  #### 7. Actual vs. Predicted Values

  #### 8. Conclusion 

  #### 9. References 




# 1. Introduction:
We developed a classification model to predict outcomes based on features. This model helps determine the likelihood of a positive result given these personal attributes.

# 2. Description of the dataset:

#### 2.1 Head of our Dataset:
The very first step is always to check if the data needs cleaning by looking for duplicate rows, zero values or NaNs where they shouldn't be etc. The head of our dataset looks like:

![test1](https://github.com/Mervin50/ML_Project3_Heart_Failure_Classification/assets/167336864/25def6ab-a768-43ac-afdd-c584ea5f1b63)


#### 2.2 Tail of our Dataset:
The tail of our dataset looks like : 

![test2](https://github.com/Mervin50/ML_Project3_Heart_Failure_Classification/assets/167336864/410d5783-efb6-49b3-a15d-492a8ef77f4b)


Visually, we found out that there are few NaN values in our dataset


# 3. Preprocessing and Data Cleaning for EDA

#### 3.1 Detecting Null values in our dataset:

![test3](https://github.com/Mervin50/ML_Project3_Heart_Failure_Classification/assets/167336864/9a73988e-e26d-4e9b-94db-4253fb3e92b1)

There are 2 each null values in Smokes and Alkhol columns. There is one null value in Age column. 

#### 3.2 Evaluating the best technique for handling null values:

![test1](https://github.com/Mervin50/ML_Project3_Heart_Failure_Classification/assets/167336864/b477e4eb-27a5-4e84-a3ef-cfc98938a7d6)

Plot is left skewed, hence we will use median technique for age column.

![test2](https://github.com/Mervin50/ML_Project3_Heart_Failure_Classification/assets/167336864/64a98d03-26b1-415f-a80e-a03892b6c85f)

Plot is right skewed, hence we will use median technique for Smokes column.

![test3](https://github.com/Mervin50/ML_Project3_Heart_Failure_Classification/assets/167336864/6b7e85f0-c10d-4bf5-b24c-a83d30f24a65)

Plot is slightly left skewed, hence we will use median technique for Alkhol column.

#### 3.3 After Treating Null values:

![test1](https://github.com/Mervin50/ML_Project2_LungCancer_Classification/assets/167336864/21b08ffb-e135-4110-8327-5b1fcae24ba5)

We have replaced our null values with median values in three columns : Age, Smokes and Alkhol

#### 3.4 Assessing Dataset Balance: 

![test1](https://github.com/Mervin50/ML_Project2_LungCancer_Classification/assets/167336864/7fdb2e12-a8d0-4743-b83f-bc26df76f5dd)

We have ratio of 32-29, so its fairly balanced dataset, so no further action is needed to balance the dataset

#### 3.5 Label Encoder:

![test1](https://github.com/Mervin50/ML_Project2_LungCancer_Classification/assets/167336864/02431943-2216-41dd-8d5c-fecb38b6e757)

We applied Label Encoder as we are solving classification problem and it helps for our model for better prediction. Label Encoder to transform categorical data into numerical form.
