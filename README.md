# **Credit Risk Analysis**

### Overview of the Analysis

For this project we use data preparation, statistical reasoning, and we applied different machine learning models to analyze credit card risk for a dataset from Lending Club. With the use of different libraries, we were able to create and obtain results with a variety of algorithms fed into each machine learning model.

We oversampled the data using the **RandomOverSampler** and **SMOTE** algorithms, and undersample the data using the **ClusterCentroids** algorithm. Then we used a combinational approach of over- and undersampling using the **SMOTEENN** algorithm. Next, we compared the two machine learning models that reduce bias, **BalanceRandomForestClassifier** and **EasyEnsembleClassifier**, to predict credit risk. (Module 18 Challenge)

### Results

The first machine model was done with the Naive Random Oversampling algorith shown below.

![Naive Random Oversampling](https://user-images.githubusercontent.com/111472338/217432859-b5d0d8d1-8a84-4ab6-ab8f-4f9e15360b4d.png)

For the NaiveRandom Oversampling Model the calculated balanced score was of 0.64 (rounded-up)

The second one was with the SMOTE algorith and here are the results

![SMOTE Oversampling](https://user-images.githubusercontent.com/111472338/217433041-882601f3-ec4c-40b2-9c81-4c54fa06e76f.png)

While the SMOTE Oversampling model showed a similar balanced accuracy score of 0.63 (rounded-up)

Then when combining both under- and over-sampling with SMOTEENN we obtained the following results

![SMOTEENN](https://user-images.githubusercontent.com/111472338/217433145-a9e8cd52-449d-4942-b9a5-e37d69cf326b.png)

The SMOTEENN calculated balanced accuracy score was of 0.63 (rounded-up); while the use of the combination (Over and Under) Sampling gave an even lower result for the calculated accuracy score of 0.52 (rounded-up)

![Combination Sampling](https://user-images.githubusercontent.com/111472338/217433158-b3c603f0-13fb-4594-98c9-88a58311d790.png)

Finally, the BalanceRandomForestClassifier and EasyEnsembleClassifier's results, respectively, are as follows

![Balance Random Forest Classifier](https://user-images.githubusercontent.com/111472338/217433294-df778916-0dcb-4a37-b8a5-8e3a08c018d1.png)

![Easy Ensemble Classifier](https://user-images.githubusercontent.com/111472338/217433317-433253f2-9bfd-4f14-8c01-5f66e07376aa.png)


### Summary

According to the results shown above along with each accuracy score for each model, the models show to have a 0.01 precision rate at "High-Risk" and a precision rate of 1.00 at "Low-Risk". 
Out of all models, **EasyEnsembleClassifier** prove to have the best reults with an accuracy rate of 0.92 (or 92%); recall or sensitivity rate of 0.94 (or 94%); f1 at a rate of 0.97 (or 97%). When predicting the candidates with highest-risk we can make the recommendation that this model be used for further analysis of the data.
