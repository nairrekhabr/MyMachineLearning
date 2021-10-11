# MyMachineLearning
Machine learning project
Credit Risk Analysis

Overview of the analysis:

The purpose of this analysis is to test the performance of several different classification models on the unbalanced loan dataset. Non-numerical columns of the dataset are transformed to categorical dummy variables, with the variable generated from each first category dropped (since their information can be deterministically inferred from the other dummie variables). The goal is to test whether a model can distinguish high-risk loans from low-risk ones given some related information.

Results:

6 models are tested and the results are summarized below:

logistic regression on random oversample :
balanced accuracy score: 0.6659
precision for high-risk/ low-risk: 0.01/ 1.00
recall for high-risk/ low-risk: 0.73/ 0.60
logistic regression on SMOTE oversampling :
balanced accuracy score: 0.6553
precision for high-risk/ low-risk: 0.01/ 1.00
recall for high-risk/ low-risk: 0.62/ 0.69
logistic regression on random undersample :
balanced accuracy score: 0.5574
precision for high-risk/ low-risk: 0.01/ 1.00
recall for high-risk/ low-risk: 0.60/ 0.51
logistic regression on combined over-undersampling :
balanced accuracy score: 0.6502
precision for high-risk/ low-risk: 0.01/ 1.00
recall for high-risk/ low-risk: 0.73/ 0.57
balanced random forest classifier :
balanced accuracy score: 0.7790
precision for high-risk/ low-risk: 0.03/ 1.00
recall for high-risk/ low-risk: 0.68/ 0.88
easy ensemble classifier :
balanced accuracy score: 0.9318
precision for high-risk/ low-risk: 0.09/ 1.00
recall for high-risk/ low-risk: 0.92/ 0.94
Summary:

In sum, the easy ensemble classifier has the best overall performance among the 6 models, and should be considered as the recommended one under this scenario.
