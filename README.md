# Spam Detection Model
This code is an example of using a Logistic Regression and Random Forest Classifier models to detect spam emails. The data used is from UCI Machine Learning Library and is located at https://static.bc-edx.com/mbc/ai/m4/datasets/spam-data.csv. The dataframe once loaded in and with the target column dropped looks like this: 

![image](https://github.com/emaynard10/Spam-Detection-Model/assets/99676466/4f25d6a5-bba7-4472-a42f-c8f60663351a)


## Technologies Used
Python, Pandas, Jupyter Notebooks, SKLearn

## Goal
The dataset contains information about emails, with two possible classifications: spam and not spam.  The  goal is to take this dataset and develop a supervised machine learning model that will accurately detect spam emails, so it can filter them out of customers' inboxes.

## Steps
1. Retrieve the Data: The data is imported using Pandas and displayed to confirm the import was successful.
2. Predict Model Performance: A prediction is made as to which model will perform better.
3. Split the Data into Training and Testing Sets: The data is split into training and testing sets, and the labels set (y) and features DataFrame (X) are created.
4. Scale the Features: The StandardScaler is used to scale the features data.
5. Create and Fit a Logistic Regression Model: A Logistic Regression model is created, fit to the training data, and tested with the testing data. The model's accuracy score is printed.
6. Create and Fit a Random Forest Classifier Model: A Random Forest Classifier model is created, fit to the training data, and tested with the testing data. The model's accuracy score is printed.
7. Determine which features are most important.
8. Plot the important features. View plot
9. Evaluate the Models: Compare the two models. The Random Forest Classifier performed better, which is as predicted. 

## Usage
The better RandomForest model could be used to weed out spam in inboxes. The RF model's accuracy is 95.6%, which is better than the Logistic regression model which had 92% accuracy. The model shows that some of the most important features include special characters and words like remove. The important features are plotted here:
![image](https://github.com/emaynard10/Spam-Detection-Model/assets/99676466/0ecffea6-8fef-475c-9366-64be3f825e34)


## Futuer Considerations
The model for this project did not require considerations of model optimization or imbalanced data. These could be taken into account for future model developement. The project uses accuracy score to determine the success of the model, but other metrics could also be considered. In this case we would want to maximize the precision of the spam(1) and maximize the recall of non spam (0). 
