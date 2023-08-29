# Spam Detection Model
This code is an example of using a Logistic Regression and Random Forest Classifier models to detect spam emails. The data used is from UCI Machine Learning Library and is located at https://static.bc-edx.com/mbc/ai/m4/datasets/spam-data.csv. The dataframe once loaded in: 
![image](https://github.com/emaynard10/Spam-Detection-Model/assets/99676466/160402f3-47db-4956-a718-24ea4858657f)

## Prediction
I predicted the Random Forest Classifier would do better than the Logistic Regression model. Due to the large number of features in the data, the random forest might do a better job with some feature selection and reducing the noise from variables that are less important. There will be a higher chance of overfitting, with higher false and true positives.


## Technologies Used
Python, Pandas, Jupyter Notebooks, SKLearn

![image](https://github.com/emaynard10/Spam-Detection-Model/assets/99676466/89589665-7779-4aa1-bdc4-862ffcef887e)


## Goal
The dataset contains information about emails, with two possible classifications: spam and not spam.  The  goal is to take this dataset and develop a supervised machine learning model that will accurately detect spam emails(spam (1) or not (0), so it can filter them out of customers' inboxes.

## Steps
1. Retrieve the Data: The data is imported using Pandas and displayed to confirm the import was successful.
2. Predict Model Performance: A prediction is made as to which model will perform better.
3. Split the Data into Training and Testing Sets: The data is split into training and testing sets, and the labels set (y) and features DataFrame (X) are created.
   
   ![image](https://github.com/emaynard10/Spam-Detection-Model/assets/99676466/69edf5d3-7c02-4e2e-afbc-894c1d96b7cc)

   ![image](https://github.com/emaynard10/Spam-Detection-Model/assets/99676466/1490e970-38f1-4592-8e96-479ff80c2445)

5. Scale the Features: The StandardScaler is used to scale the features data.
   ![image](https://github.com/emaynard10/Spam-Detection-Model/assets/99676466/36eaa593-e2c9-4483-bcbf-f26ef5141dc2)


7. Create and Fit a Logistic Regression Model: A Logistic Regression model is created, fit to the training data, and tested with the testing data. The model's accuracy score is printed. Accuracy Score :   0.9226759339704604

   ![image](https://github.com/emaynard10/Spam-Detection-Model/assets/99676466/7caa2b31-f899-469f-92a6-d47c21a13568)

9. Create and Fit a Random Forest Classifier Model: A Random Forest Classifier model is created, fit to the training data, and tested with the testing data. The model's accuracy score is printed. Accuracy Score : 0.9565595134665508

   ![image](https://github.com/emaynard10/Spam-Detection-Model/assets/99676466/029f49a8-f1ab-4aa9-afed-306f12ac2d9b)

11. Determine which features are most important.

   ![image](https://github.com/emaynard10/Spam-Detection-Model/assets/99676466/e40c0e6d-66c2-41aa-8ccd-58b0840e07d1)


13. Plot the important features. View plot

    ![image](https://github.com/emaynard10/Spam-Detection-Model/assets/99676466/7ac6018c-0354-4f90-a99c-200c36eac0a9)

15. Evaluate the Models: Compare the two models. The Random Forest Classifier performed better, which is as predicted. 

## Usage
The better RandomForest model could be used to weed out spam in inboxes. The RF model's accuracy is 95.6%, which is better than the Logistic regression model which had 92% accuracy. The model shows that some of the most important features include special characters and words like remove. The important features are plotted here:
![image](https://github.com/emaynard10/Spam-Detection-Model/assets/99676466/0ecffea6-8fef-475c-9366-64be3f825e34)


## Futuer Considerations
The model for this project did not require considerations of model optimization or imbalanced data. These could be taken into account for future model developement. The project uses accuracy score to determine the success of the model, but other metrics could also be considered. In this case we would want to maximize the precision of the spam(1) and maximize the recall of non spam (0). 
