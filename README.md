# Hubble-Evolution-using-gplearn

This code demonstrates the use of symbolic regression to predict the Hubble evolution (H) with redshift (z) using a specified mathematical equation.


## AayushaDataSetPractice 

Here is a summary of the steps taken in the project:

1. Importing Necessary Libraries:
I began by importing essential Python libraries, including numpy, pandas, and gplearn.

2. Data Preprocessing:
I loaded a dataset related to kidney data and performed preprocessing to select relevant features.

3. Symbolic Regression Model:
To demonstrate the symbolic regression process, I created a sample dataset with features such as 'CAN_LAST_SRTR_PEAK_PRA', 'DON_RACE', 'DON_GENDER', and the target variable 'Avg_EMS_30'.

4. SymbolicRegressor:
Using the SymbolicRegressor class from gplearn, I created a symbolic regression model. This class allows us to define parameters like population size, generations, and mutation rates that influence the genetic programming process.

5. Data Splitting:
The data was then split into training and testing sets using train_test_split from sklearn.model_selection. The model was trained using the training set via est_gp.fit(X_train, y_train).

6. Model Evaluation:
Following the model fitting, I checked if the model was successfully fitted and predicted the target variable on the testing set. I evaluated the model's performance using mean squared error.

7. Visualization:
Lastly, I visualized the symbolic expression obtained from the model using pydot and Image from IPython.display. The symbolic expression represents the mathematical relationship discovered by the genetic programming algorithm.

8. Performance Visualization:
Additionally, I created a scatter plot comparing the actual and predicted values of 'Avg_EMS_30', demonstrating how well the model performed in capturing the underlying relationships in the data.