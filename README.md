# BoostUpClassifierPerformance
A college project to boost up classifier performance with image PCA data.

This project is part of the Business Analytics course. The data used for PCA is image data on the types of diseases in tomato plants from Kaggle https://www.kaggle.com/kaustubhb999/tomatoleaf.
This data only contains three types of tomato plant diseases, namely diseases caused by Mosaic Virus, Yellow Leaf Curl Virus, and disease Septoria Leaf Spot, with 10 photos each for every disease in th preliminary data. These three types of disease are represented by spots or shapes which is unusual on the leaves.

The aim of this project is to experiment with many techniques to boost up the performance of the classifier. At first, we used Naive Bayes for the classifier as a performance standard. The techniques are as follows:
1. Add more train data
2. Add more PC features
3. Do feature scaling
4. Change model algorithm
5. Do hyperparameter tuning

# Hypothesis
My initial hypothesis was that the low accuracy was due to too little data for training which was only 10 pieces for each type of disease. While the types of diseases that have a fairly high similarity, for example, leaves infected with Tomato Virus Mosaics and Tomato Yellow Leaf Curl Virus which both have signs of leaves turning bright yellow, the intensity of yellow in the Tomato Yellow Leaf Curl Virus is higher. So, I think the model needs more data to learn.

# Conclusion
From the experiments to improve performance on the type of disease data, it can be concluded that:
1. In accordance with the hypothesis at the beginning, in this case increasing the number of data train can be improved classifier performance, as evidenced by the initial accuracy of 33% to
83% 
2. In this case adding PC features degrades the performance of the classifier, evidenced
with an initial accuracy of 33% to 17% for data with 30 images and from 83% to 58% for the data with 60 images
3. In this case, performing feature scaling does not increase or decrease classifier performance, so it is known that the data does not have a far range and normally distributed
4. In this case, changing the model algorithm does not improve the performance classifier significantly. With 30 images of data, the Ada Boost model is better less performance than Naïve Bayes (accuracy to 50%). While the model Naïve Bayes and the Random Forest Classifier have the same accuracy with the data 30 images (33%) and 60 images (83%)
5. In this case, perform hyperparameter tuning of the data with 30 images improve classifier performance quite well, but on data with 60. Image accuracy was found to be lower than the un-tuned algorithm hyperparameter
