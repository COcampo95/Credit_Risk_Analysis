# Credit_Risk_Analysis

##Results:


Naive Random Oversampling:
![Photo_1](https://user-images.githubusercontent.com/105950742/193168478-7ec98a17-4ab7-445d-b70a-4af4fa70bc5e.png)
![Photo_2](https://user-images.githubusercontent.com/105950742/193168480-b93c02fc-3326-4beb-8faf-f0d6303cc961.png)

SMOTE Oversampling:
![Photo_3](https://user-images.githubusercontent.com/105950742/193168481-5527a2a2-ed55-46b7-9f22-85b7a5ad6e1c.png)

Cluster Centroid Undersampling:
![Photo_4](https://user-images.githubusercontent.com/105950742/193168472-68f2111d-87c0-4106-b33d-1a8384371f65.png)

SMOTEENN Combination Sampling:
![Photo_5](https://user-images.githubusercontent.com/105950742/193168473-4b404ffb-a7a1-4d19-b1d3-aead0fa51366.png)

Balanced Random Forest Classifier:
![Photo_6](https://user-images.githubusercontent.com/105950742/193168475-d4a52e5d-52c3-4443-b54a-1dca88374a35.png)

Easy Ensemble AdaBoost Classifier:
![Photo_7](https://user-images.githubusercontent.com/105950742/193168476-9e3360cf-c3d4-40b8-8563-e39e6aa41975.png)


##Summary:
For precision, all six algorithms had a really low precision rate for high risk individuals. The highest one was the Easy Ensemble AdaBoost Classifier with 7% precision which is still considered pretty low for finding these high risk individuals not to give loans to. This means that out of all the customers marked as high-risk 7% were actually high-risk. On the other hand, all the models had a perfect precision for low-risk individiauls meaning that all of the low-risk customers were marked as that.

Having this in mind, precision is not telling us much information to compare the algorithms, so we should take a look at sensitivity. The model with the highest sensitivity was the easy ensemble adaboost classifier (91% for high-risk and 94% for low-risk individuals), meaning that 91% of the time all the high-risk individuals are marked as high-risk individuals. Followed by this model, the other two with high recall were the Random Forest Classifier (67%) and SMOTEENN Resample (70%).

And last but not least, we are going to look at the balanced accuracy score to make the final decision of which model to use. The accuracy score stands for how correct was the model, meaning out of all the predictions how many of them were true to the classification. As we were able to see, the model with the highest accuracy score by far was the Easy Ensemble AdaBoost Classifier. So, this should be the one we chose because of its high accuracy, highest precision, and highest sensitivity.
