EDA : 

the dataset name : data 

for columns (Partner,Dependents,PhoneService,PaperlessBilling,Churn) :
    1 : Yes
    0 : No

We used One-hot encoding for those columns : (PaymentMethod,Contract,StreamingMovies,
StreamingTV,TechSupport,DeviceProtection,OnlineBackup,OnlineSecurity,InternetService,
MultipleLines)

for Gender column :
    1 : Male
    0 : Female

We created a mapping dataset to store costumers Ids to use them is needed to look directly 
for the data of a user

the column TotalCharges had object as dtype which won't work in the pahse of training so we
transformed it into numerical type

y being the output churn 

x being data but without y 

we devised the data into test/train datasets with ( test dataset fraction = 20%)


ML : 

we train linear regression and logistic regression models on y_train and x_train

then we use >0.5 filter to turn continous values of linear model to be binary 

then we use metrics (precision , recall , acurracy and F1 score) to evaluate each of the models

the results confirmed that logistic regression did better than logostic regression 


