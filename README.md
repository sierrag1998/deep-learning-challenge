# Unit 21 Homework: Charity Funding Predictor

## About the Repository 
Included in this repository are 4 jupyter notebook. The original model is built in Starter_Code.ipynb. There are 3 attempts at optimizing the model included in Optimization_One.ipynb, Optimization_Two.ipynb, and Optimization_Three.ipynb.

The saved HDF5 files from each notebook are included in the Saved Model Folder. The original data set is included in the Resources Folder. The report on the assignment is included in the Optimizing Alphabet Soup PDF, and the rubric is included in the Module 21 PDF for ease of access. 


## About the Assignment 

Using the data set given, I created a binary classifier model that can predict whether applicants will be successful if funded by Alphabet Soup.



### Step 1: Preprocess the Data


### Step 2: Compile, Train, and Evaluate the Model


### Step 3: Optimize the Model


### Step 4:  Report on the Neural Network Model


Optimizing Alphabet Soup
Overview: The purpose of this analysis is to create a binary classifier
that can predict whether an applicant will be successful if funded by
Alphabet Soup. This analysis will help Alphabet Soup make better,
more informed decisions when deciding which applicants to approve.
Results:
Data Preprocessing:
The target variable in the model is whether the application
“IS_SUCCESSFUL” shown by a binary score in the “IS_SUCCESSFUL”
column of the dataset.
The feature variables are the application type, the affiliated sector, the
government organization classification, the use case for funding, the
organization type, the status, the income amount, the ask amount,
and special considerations. These are identified by the following
columns. ['APPLICATION_TYPE', 'AFFILIATION', 'CLASSIFICATION',
'USE_CASE', 'ORGANIZATION', 'INCOME_AMT',
'SPECIAL_CONSIDERATIONS']
There were two identification columns “EIN and NAME” that were
removed from the dataset as they were neither targets nor features.
Compiling, Training, and Evaluating the Mode:
I had 3 layers (2 hidden, and output layer). The activation function are
RELU on the first two and sigmoid on the output layer. The first layer
has 8 neurons and the second layer has 5 neurons. These choices
were made due to experimentation with different numbers and layers
and this was the highest accuracy combination.
While close, I was not able to reach target model performance as the
accuracy score was 72.46%. I created 3 different attempts to
optimize my model. In my first attempt, I did not filter out values out
of the application and classification types. The resulting accuracy of
this model was slightly lower at 72.33%.In the second attempt, I
increased the neurons in my first and second hidden layer from 8 and
5 to 10 and 12. The resulting accuracy of this model was slightly
higher at 72.51%.In my third attempt, I added an additional hidden
layer with 14 neurons and sigmoid activation layer.
The resulting accuracy of this model was slightly higher at 72.72%.
Summary: Overall, I got the highest accuracy level during my third
attempt. A model with more hidden layers could possibly provide a
higher accuracy score. This is recommended based on the fact that
this dataset has a high number of features.
![image](https://user-images.githubusercontent.com/105753641/202873141-1c7b7985-47db-4c49-afc2-388dd841105a.png)
![image](https://user-images.githubusercontent.com/105753641/202873154-7f8af715-ad12-4515-92a4-449c1ee5067b.png)
![image](https://user-images.githubusercontent.com/105753641/202873164-d27db1af-828c-41d8-b20c-d410b47a7f16.png)

