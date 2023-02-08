# **Credit Risk Analysis**

### Overview of the Analysis

For this project we use data preparation, statistical reasoning, and we applied different machine learning models to analyze credit card risk for a dataset from Lending Club. With the use of different libraries, we were able to create and obtain results with a variety of algorithms fed into each machine learning model.

We oversampled the data using the **RandomOverSampler** and **SMOTE** algorithms, and undersample the data using the **ClusterCentroids** algorithm. Then we used a combinational approach of over- and undersampling using the **SMOTEENN** algorithm. Next, we compared the two machine learning models that reduce bias, **BalanceRandomForestClassifier** and **EasyEnsembleClassifier**, to predict credit risk. (Module 18 Challenge)

### Results

The first machine model was done with the Naive Random Oversampling algorith shown below.

![Naive Random Oversampling](https://user-images.githubusercontent.com/111472338/217432859-b5d0d8d1-8a84-4ab6-ab8f-4f9e15360b4d.png)

The second one was with the SMOTE algorith and here are the results

![SMOTE Oversampling](https://user-images.githubusercontent.com/111472338/217433041-882601f3-ec4c-40b2-9c81-4c54fa06e76f.png)

Then when combining both under- and over-sampling with SMOTEENN we obtained the following results

![SMOTEENN](https://user-images.githubusercontent.com/111472338/217433145-a9e8cd52-449d-4942-b9a5-e37d69cf326b.png)

![Combination Sampling](https://user-images.githubusercontent.com/111472338/217433158-b3c603f0-13fb-4594-98c9-88a58311d790.png)

Finally, the BalanceRandomForestClassifier and EasyEnsembleClassifier's results, respectively, are as follows

![Balance Random Forest Classifier](https://user-images.githubusercontent.com/111472338/217433294-df778916-0dcb-4a37-b8a5-8e3a08c018d1.png)

![Easy Ensemble Classifier](https://user-images.githubusercontent.com/111472338/217433317-433253f2-9bfd-4f14-8c01-5f66e07376aa.png)


### Summary

According to the results shown above, the dataset for credit card risk provided by Lending Club is the Easy Ensemble AdaBoost Classifier with an accuracy of 93% or 0.93 (closest to one); and with a recall score of 94% or 0.94. Based on our findings we can confidently say that this is the best approach to continue to explore and do further analysis in this data with.
