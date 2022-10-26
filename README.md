# Credit_Risk_Analysis

## Overview

Credit risk is difficult to predict. For this project we will analyze how all the factors in our loan_stats csv file help predict wheather an individual has a high or low credit risk. We will create models using imbalanced-learn and scikit-learn libraries. Then we will evaluate those models using resampling methods such as oversample and undersample. In the first few models we oversampled the data using randomoversampler and smote algorithms and undersample the data with the clustercentroid algorithm. For the remaining models, we used a combination approach to oversample and undersample the data using the smoteenn algorithm. Finally, we compared 2 machine learning models that minimize bias.

## Results:

#### Naive Random Oversampling: 
Our balanced accuract test is 65%, the precision for the high risk loans has a low positivity of 1% and the recall is 61%

![Screenshot_20221026_061505](https://user-images.githubusercontent.com/106443196/198149472-b91c4dac-25ac-4fd6-b2b7-0fba19d9ce90.png)

#### SMOTE Oversampling: 
Our balanced accuracy test is 64.6%, the precision for the high risk loans has a low positivity of 1%  and the recall is 66%

![Screenshot_20221026_062345](https://user-images.githubusercontent.com/106443196/198150013-63630e9a-27f6-40fb-a4af-e5958105a3d7.png)

#### Undersampling:
Our balanced accuracy test is 51%, the precision is 99% and the recall is 44%

![Screenshot_20221026_062628](https://user-images.githubusercontent.com/106443196/198150336-ccd741bc-e4e2-4323-9c7e-7e24c5b79e48.png)

#### Combination (Over and Under) Sampling:
Our balanced accuracy test is 62.7%, the precision is 99% and the recall is53% overall combination

![Screenshot_20221026_063002](https://user-images.githubusercontent.com/106443196/198150810-474515d9-5f51-41e5-a1e3-ae6b4b0fc4f8.png)

#### Balanced Random Forest Classifier: 
Our balanced accuracy test is 76.5%, the precision is 99% and the recall is 89%

![Screenshot_20221026_063404](https://user-images.githubusercontent.com/106443196/198151597-74a4aa01-b1b9-4196-95be-1c4fd5a92a94.png)

#### Easy Ensemble AdaBoost Classifier:
Our balanced accuracy test is 91.7%, the precision is 99% and the recall is 94%

![Screenshot_20221026_063744](https://user-images.githubusercontent.com/106443196/198151941-4e1ccf7c-2ca5-4967-a778-2c3cf02873dd.png)

## Summary

In the first 4 models we undersampled, oversampled and a combination of both in order to determine which model is best at predicting which loans are the highest risk. The following 2 models we resampled the data using ensemble classifiers in order to predict which loans are high or low risk. The accuracy score for the first 4 models was not as high as the ensemble classifiers and the recall in the oversampling, undersampling, and mixed models is low. In order to maintain a good balane of recall and precision we recommend the ensemble classifiers over the first 4 models. The Easy Ensemble proved to have the best balance of all the models because of it's high accuracy score, precision and recall scores.
