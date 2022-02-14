# ML-Digit-Recognizer-Kaggle

Get my notebook: https://colab.research.google.com/drive/153z1NtfiESG3e7YJNUQC8hEN5-U28pjN?usp=sharing

I. Introduction: Research Question and Problem for Management

The digit recognizer dataset consists of 754 attributes, all of which are pixels for an image of a number 0 through 9. The purpose of this study is to create a model that is able to predict which number will be displayed by the image given a 0 or 1 for each pixel. Providing a model for the digit recognizer is an example of how unsupervised learning can be used for visual data. 

II. Analysis of Dependent Variable (label - 0 through 9 image)

An initial analysis of the dependent variable 'label' shows that this data consists of images of the numbers 0 through 9. The training dataset has 42,000 images encoded by pixel number and the test dataset has 28,000 instances of pixel data that can be used to predict the number label. Each of the numbers had fairly consistent samples, ranging from 3795 instances to 4684 instances per number. A plot of the counts for each number label can be seen in Figure 1. 

![image](https://user-images.githubusercontent.com/97359451/153781205-c5cc781f-2e73-46c8-bd80-9f31afc6786f.png)
Figure 1. Histogram of counts per label for the training dataset.


IV. Models

The first model to be tested was a random forest after the training set was split between pixel variables and the dependent variable 'label'. The Random forest classifier took 31.94 seconds to fit the data and after predicting the test dataset, it was 96.546 correct in predicting the number labels of the dataset. After the initial random forest classifier model was created, a principal component analysis was completed to determine which pixels would be used in the component model. After applying the pca, the random forest model given those components performed at 94.35 percent accuracy on predicting the test dataset labels. Finally, a k-means model was used to predict the test dataset which performed worse than either random forest with accuracy of 89.83%.


VII. Conclusions

After testing several models, the original random forest model performed the best on the testing data. All pixels were included in this model and it performed with 96.546% accuracy. The model can be improved by parameter testing and improving the principal component analysis to get a more accurate set of components to fit on the model. 
