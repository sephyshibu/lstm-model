# lstm-model
we are detecting the COVID-19 cases, i.e., positive cases,death cases,total death
cases,total cases We are performing this analysis based on the cases in chronological dates.
On this dataset, first, we performed data cleansing and feature selection, then performed
forecasting of positive cases using Long Short term Memory(LSTM), Bidirectional LSTM
where Bidirectional LSTM outperformed the others, therefore, the Bidirectional LSTM is
used for prediction and analysis of all the results. Predicted patients are also compared with
a prediction model for the same duration, and results revealed that the predicted patients’
count of the proposed model is much closer to the actual patient count.

 This article has used long short-term memory (LSTM) and Bidirectional LSTM to predict the COVID-19
positive patients in India. LSTM is a particular type of recurrent neural network (RNN) used
for classification, prediction, and regression tasks.Two connected layers are used to process
the input data. Each layer performs the operations using reversed time step direction.Bi-
directional Recurrent Neural Networks are used to learn from both the forward and backward
time dependencies. We have trained the model on Covid-19 data (30 January 2020 to 11
August 2021) of India and predict the Covid positive patients
Finally, we have calculated the accuracy and compare each model to find the maximium
accuracy of different states of India and results revealed that the predicted patients’ count of
the proposed model is much closer to the actual patient count.

Data cleaning means two things: (i) correcting/addressing any mistakes in the data (ii)
organising the data in ways to help the downstream analysis e.g., clearer variable names,
factor levels, data transformation. In this dataset using mean imputation to fill all the missing
values.where the missing value is replaced with the sample mean. This preserves the estimate
of central tendency but at the expense of deflating the estimate of variance. This is potentially
problematic especially when many values are imputed.

**Feature Selection**
During the process of model building, feature selection is used to select most relevant
features out of all the features. It reduces the complexity of the prediction model.Correlation
is meant for exploring the degree of relationship between two variables in consideration.
Correlation coefficient is the measure to quantify such degree of relationship of the variables.
Generally, two correlation coefficients are used in applications, namely: Pearson’s Product
Moment Correlation Coefficient and Spearman’s Rank Correlation Coefficient.If the trend
of a variable is positive and almost similar to another variable, there may be possibility to
have positive association of each other and such association can provide positive correlation
coefficient; and If the trend of a variable is positive and almost negative to another variable,
there may be possibility to have negative association of each other and such association can
result in negative correlation coefficient.Here have 2 correlated features out of 6 features.The
coorelated features are Confirmed, Death.


**Algorithm**
Input: COVID 19 Dataset
Output: Graph representing test and predicted values
Prerequisites: Import required libraries
split() : split given array in two parts
N : LSTM Network
E : Number of epochs
Batch-size : N
D ← read(data)
traindata, testdata ← split(D)
K ← G(traindata)
L ← G(testdata )
LSTM
Initialize layers,input shape, optimizer and loss function to define N.
for k = 1 to E do
Train(N, K);
end for
P ← predictions(N, L)
Graph(testdata , P)
Bidirectional LSTM
Initialize layers,input shape, optimizer and loss function to define N.
for k = 1 to E do
Train(N, K);
end for
P ← predictions(N, L)
Graph(testdata , P)

