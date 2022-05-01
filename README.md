# Credit_Risk_Analysis

## Overview of the loan prediction risk analysis:

Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans.We will oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, we will use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Then, we will evaluate the performance of these models. 


## Results:

1. Naive Random Oversampling

Balanced Accuracy Score: The accurately predicts credit risk 63.6% of the time when the minority class is balanced by oversampling.
Preciscion: The precision of this model is 0.01 for high risk and 1.00 for low risk applicants. This means that 100% of the predicted low risk applicants are actually low risk, but only 1% of the predicted high risk applicants are actually high risk.
Recall: The recall of this model is 0.65 for high risk, and 0.62 for low risk applicants. 

![Naive Random Oversampling](https://user-images.githubusercontent.com/95401877/166134005-30db4f6a-4afb-4e94-be33-fe199da8f0b5.jpg)

2. SMOTE Oversampling

Balanced Accuracy Score: The accurately predicts credit risk 63.07%, it is lower than NRO model.
Preciscion: The precision of this model is 0.01 for high risk and 1.00 for low risk applicants. This model has no difference with NRO model.
Recall: The recall of this model is 0.62 for high risk, which lower than NRO model, but 0.64 for low risk applicants is higher than NRO model. 

![SMOTE Oversampling](https://user-images.githubusercontent.com/95401877/166134348-cac2fa4b-590a-4064-a04a-c7d508c48eea.jpg)

3. Undersampling

Balanced Accuracy Score: The accurately predicts credit risk 51.6%, it is lower than other models.
Preciscion: The precision of this model is 0.01 for high risk and 1.00 for low risk applicants. This model has no difference.
Recall: The recall of this model is 0.60 for high risk and 0.43 for low risk applicants is lower than other models. 


![Undersampling](https://user-images.githubusercontent.com/95401877/166134435-bc8b3732-796b-42b2-982b-3ee8347deb9d.jpg)

4. Combination (Over and Under) Sampling

Balanced Accuracy Score: The accurately predicts credit risk 62.5%.
Preciscion: The precision of this model is 0.01 for high risk and 1.00 for low risk applicants. This model has no difference.
Recall: The recall of this model is 0.71 for high risk is higher than others, and 0.59 for low risk applicants. 

![Combination (Over and Under) Sampling](https://user-images.githubusercontent.com/95401877/166134791-3c8ecae9-0fe5-48d2-b53c-77efc502c6f7.jpg)

5. Balanced Random Forest Classifier

Balanced Accuracy Score: The accurately predicts credit risk 78.8%
Preciscion: The precision of this model is 0.07 for high risk and 1.00 for low risk applicants. This model has different high risk.
Recall: The recall of this model is 0.91 for high risk is higher than others, and 0.94 for low risk applicants. This ensemble model a better performer than models built from sampling techniques alone.

![Balanced Random Forest Classifier](https://user-images.githubusercontent.com/95401877/166134946-3a3a7d1b-6c75-4ef9-b028-6c7f518f7c09.jpg)

6. Easy Ensemble AdaBoost Classifier

Balanced Accuracy Score: The accurately predicts credit risk 92.5%, when multiple models are trained sequentially on a balanced dataset to minimize error.
Preciscion: The precision of this model is 0.09 for high risk and 1.00 for low risk applicants. This model has different high risk.
Recall: The recall of this model is 0.92 for high risk is higher than others, and 0.94 for low risk applicants. This ensemble model is also a better performer.

![Easy Ensemble AdaBoost Classifier](https://user-images.githubusercontent.com/95401877/166135303-a55577dd-10c3-4fb9-88fc-5cb044c09dfc.jpg)


## Summary:

All the models have the downside, but from overall "Easy Ensemble AdaBoost Classifier" is a best 
