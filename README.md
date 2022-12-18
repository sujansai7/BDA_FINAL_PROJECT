# Deliverable 1

# 1. Team

## Project Group # 23

## a) Members

•	Noolu Sai Sujan
•	Rimjhin Jain
•	Avinash Kamatham
•	Nandakishore
•	Mounika Kasargadda

## b) Communication plan to include project artifact repository, meeting notes, meeting platform, etc.

Github Repo, Email communication, Slack

# 2. Selection of data (https://www.kaggle.com/datasets/ekibee/car-sales-information)

This is a dataset with data on car sales ads in Russia by region

Description: Data for car sales ads in Russia

Resource type: S3 Bucket

Amazon Resource Name (ARN): arn:aws:s3:::checkcheckbucket

AWS Region: US-global

https://github.com/sujansai7/BDA_FINAL_PROJECT

# 3. Business Problem or Opportunity, Domain Knowledge

The dataset we have chosen is from Kaggle where it has been collected from a popular website in Russia with ads for the sale of cars, the dataset is frequently updated on a weekly basis it contains information related to cars in over 18 columns among which it has columns like price of the car, brand name, fuel type, colour, mileage, power etc. We can use this data to derive some useful information like what price range people are most interested to buy in, what kind of colour people like the most irrespective of the price, what kind of fuel typed cars are given most importance, and also understand the correlation between different variables that are tightly related using correlation graph so it gives us which variables in the dataset are closely related so that they can be given more importance.

# 4. Research Objectives and Question(s)

There have been several questions which arise during my research work. The following questions mentioned below are some of the questions which are needed to be researched in depth and should be discussed at a bigger prospective.

•	Which fuel type vechicles are having higher priority? 

•	What is the price range that most of the customers are willing to buy ?

•	What body type vehicles are much preferred?

•	What kind of transmission are the customers purchasing most?


# Deliverable 2

# Data Understanding
## a) Exploratory Data Analysis
Exploratory Data Analysis was done through AWS Sagemaker. The link for the file is pasted here:
https://github.com/sujansai7/BDA_FINAL_PROJECT/blob/4768cee13a8cc3bcbb6b5b4d7ea616f9cf02bf47/BIG_DATA_PROJECT.ipynb

## b) Dashboard
Dashboard instances were created using AWS Quicksight. These dashboards are used for presenting results using visualizations such as representing graphs like Pie Chart and Bar Chart for evaluating the research objectives. Also several different plots have been created using Scikit learn library from python and Amazon SageMaker notebook (AWS).
Some of the graphs for AWS QuickSight are presented in the PDF, the link for the same is pasted below:

https://github.com/sujansai7/BDA_FINAL_PROJECT/blob/main/AWS_QuickSight.pdf

# Data Preparation
As part of the data preparation process, all null values are first checked since they limit the ability of the machine learning algorithm to learn. Each column's null values are examined, and all of them are replaced with zero. After completing the above step, the data on each column was carefully observed and the Standard deviation, Mean, Maximum, and other statistical distributions are examined to determine how evenly the data is distributed.
The string values present in columns are then transformed into integers as the machine learning algorithm cannot takes string values as input for processing.

# Deliverable 3
 

# Analytics, Machine Learning

Amazon Machine Learning technologies like SageMaker are used for analytics and machine learning. The data was originally recognized using Amazon Athena and Glue before being worked on by SageMaker. To use the best ML tools on the dataset's structure and get the most accurate results, the dataset's schema is thoroughly examined. The Amazon SageMaker is used finally to get the results.
The data recognition is presented below:

<img width="452" alt="image" src="https://user-images.githubusercontent.com/115503621/207416834-3bfefc5e-464c-437a-b79a-eeb5fa505d1c.png">

<img width="452" alt="image" src="https://user-images.githubusercontent.com/115503621/207416853-30dbd38c-7af7-4ba8-a904-30a7b22f6655.png">

<img width="452" alt="image" src="https://user-images.githubusercontent.com/115503621/207416876-fe2d3175-e788-4df5-8abc-2c28c261e4ef.png">

<img width="452" alt="image" src="https://user-images.githubusercontent.com/115503621/207416912-baf17c53-d07d-4ef2-8f8c-51ded5aabbe0.png">
 
# 8. Evaluation and Optimization
AWS offers a variety of machine learning models and analytic tools, but linear regression was chosen as it offers outstanding approach to demonstrate patterns and relations across datasets. Linear regression attempts to model the relationship between two variables by fitting a linear equation to observed data. One variable is considered to be an explanatory variable, and the other is considered to be a dependent variable.

# 9. Results
The results for some of the questions raised are discussed based upon proper data, performing pre-processing operations on data and including all the required parameters.The price predicted based on parameters like bofy type, fuel type is mentioned in the link below.

https://github.com/sujansai7/BDA_FINAL_PROJECT/blob/main/BigData_deliverable%203%20Code.ipynb

##  Which fuel type vehicles are having higher priority?
According to the bar graph and pie chart, it is found out that the vehicles with Gasoline (90%) as fuel type are highly preferred. The vehicles with Diesel (9%) are chosen next followed by Electro(1%). The graphs for the visualization are presented below.
 
<img width="448" alt="image" src="https://user-images.githubusercontent.com/115503621/207417083-febb611c-278d-4dd9-90a1-01955db47132.png">

<img width="316" alt="image" src="https://user-images.githubusercontent.com/115503621/207417108-a879e296-434a-40bf-9f25-d6bd36fccb0f.png">

 
## What body type vehicles are much preferred?

The graphs for the analyzation are attached below. The analysis can be described as follows:
•	The jeep 5 doors has the highest count (490000) signifies as highest preferred.
•	The hatchback door 5 has a count (27000) which is the second preference.
•	The sedan has a count (25000) followed by minivan and station wagon.
•	The least preferred is coupe body type with a count of (100000). 

The bar chart presents a clear representation of the preference scale for cars based on body type.
 
<img width="452" alt="image" src="https://user-images.githubusercontent.com/115503621/207417150-d3ed9a16-8569-41de-a2fd-a5ffdf4e994e.png">

<img width="374" alt="image" src="https://user-images.githubusercontent.com/115503621/207417167-fc685c81-1dd5-46c4-b2d2-609231377634.png">


## What kind of transmission are the customers purchasing most?
Below are the graphs representing the relation between color and body type of the car which are preferred most when combined. 

It can be estimated that:

A white color with body type as jeep 5 doors is the highest preference with a count of  170000. 

Also, the lowest preferred car is with the body type coupe including different color variations.

<img width="452" alt="image" src="https://user-images.githubusercontent.com/115503621/207417335-fa4da9a9-7414-4bdb-bf7c-a035bd1e44b5.png">

 
Below is the graph representing the fuel type and model of the car combination.
According to the graph, 

The highly preferred model is a Gasoline Toyota with a count of 60000.
 Also, there are models for which the value for count for every fuel type is negligible or zero. 
 
 <img width="452" alt="image" src="https://user-images.githubusercontent.com/115503621/207417383-6a12f4fd-cb70-4a35-bdb1-9116a0bfbd99.png">

 

## What is the price range that most of the customers are willing to buy ?
The price range is the final step evaluation as it is based on several parameters such as brand, body type, color, fuel type and many more features.
 
Based upon these features the price of the car is estimated and a list of final price is presented in the graph. 

<img width="452" alt="image" src="https://user-images.githubusercontent.com/115503621/207417438-2b83a070-3bec-46fa-a1ca-e36f54005c53.png">

 
The linear regression model is applied to check the price which are highly preferred by a customer.

A list of highly predicted values are represented below after including all the parameters.

The output for the same is present below.

<img width="452" alt="image" src="https://user-images.githubusercontent.com/115503621/207417459-36711ab3-b6cc-48cd-a6a8-121fdbbc9f26.png">


# Future Work, Comments

## What was unique about the data? Did you have to deal with imbalance? What data cleaning did you do? Outlier treatment? Imputation?
The data was unique in several factors. It included several different features which proved to be very efficient in predicting the highly preferred final price of the customers. It included null values which had to be replace with zero for better performance of machine learning models. The string values present in the dataset also created imbalances during the project and were transformed to integer values as machine learning models cannot work with strings values as inputs. The data cleaning consisted of eliminating the null values present in the dataset. The data on each column was carefully observed and the Standard deviation, Mean, Maximum, and other statistical distributions are examined to determine how evenly the data is distributed for imputation.

## Did you create any new additional features / variables?
There weren't any new variables, but there were undoubtedly a number of new features. To begin with, AWS Athena and AWS Glue were used to identify the data in the dashboards made in AWS Quicksight. During the Analytics/ML modeling phase, regression models, such as linear regression, are used to present the results of the data. AWS SageMaker was used for generating the outcomes.

## What was the process you used for evaluation? What was the best result?
A lot of AWS resources were used during the process including AWS Glue, AWS Athena, AWS Quicksight. All these platforms were used to identify and understand the data after the pre-processing of the data. The processed data is transferred to the AWS SageMaker and linear regression is performed to obtain the final results. The plots for the same are generated using matplotlib and other Machine Leraning tools to provide the answers for the research questions.

## Is there Bias in your work? What were the problems you faced? How did you solve them?
During the project creation there were several problems encountered. There was a problem with a dataset which was chosen. It had to be pre-processed to remove the null values present in the columns of the dataset. Also, the dataset chosen is a Kaggle dataset and setting up the Kaggle dataset on AWS services was a challenge. Also, there were issues while setting up AWS Glue, AWS Athena. Additionally, some of the data operations could not be set up the AWS services initially due to credits.  

## What future work would you like to do?
The future work comprises including several more related datasets to work with a variety of datasets within the same project. Also more visualization apps like Bokeh can be proved beneficial in future for better understanding of the project.
Also, the project is planned to be enhanced further to make it a real-world application with minimal errors.

## Instructions for individuals that may want to use your work
The dataset is chosen from Kaggle and anyone who wishes to use our work needs to setup the AWS environment with appropriate credentials. Also, it might ask for charges which needs to be paid before using AWS services. Also, the user must load the Kaggle data into AWS and then set up the AWS SageMAker to run the python notebook consisting of code. All the other requirements for the procedure is mentioned within the github repository.

# Implementation of Work / Presentation Video

Deliverable 1: https://github.com/sujansai7/BDA_FINAL_PROJECT/blob/main/Deliverable1.mp4

Deliverable 2: https://github.com/sujansai7/BDA_FINAL_PROJECT/blob/main/Deliverable2%20.mp4

Deliverable 3: https://github.com/sujansai7/BDA_FINAL_PROJECT/blob/main/Deliverable3.mp4
