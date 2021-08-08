__Title:__ Detecting Parkinson’s Disease by Machine Learning using XGBoost Algorithm

__Abstract:__

Parkinson’s Disease (PD) is a slowly progressive chronic neurologic condition which causes a gradual loss of the nerve cells in the brain. Roughly six million people worldwide suffer from Parkinson’s disease. Hyperparameter optimization was performed on the XGBoost algorithm machine learning model for the UCI ML Parkinson’s disease dataset which contains features extracted from 195 sustained vowel phonations from 31 male and female subjects, of which 23 were diagnosed with PD. This model was able to predict Parkinson's disease with 100% accuracy on the testing dataset, i.e., no false positive or false negative result was predicted.

__Introduction:__

Parkinson’s disease is second only to Alzheimer’s disease as the most prevalent neurodegenerative disease worldwide. (Reference 1) Despite extensive research, there is no known cause, cure, or prevention for Parkinson’s disease but the symptoms can be alleviated significantly with medication especially if correct diagnosis is obtained at the early stage of the disease. Little et al. from University of Oxford published a study on the Suitability of Dysphonia Measurements
for Telemonitoring of Parkinson’s Disease in 2008 where they were able achieve overall correct classification performance of 91.4%, using a kernel support vector machine. (Reference 2) In this study the default parameters for the XGBoost Classifier Model yielded an accuracy of 94% and after hyperparameter tuning the accuracy went up to 100%. 

__Methodology:__

1. The data file (parkinsons.data) was downloaded from UCI Machine Learning Databases. (Reference 3)
2. A pandas DataFrame was created from the data file.
3. DataFrame was checked for any duplicates and missing values.
4. DataFrame was plotted in a scatter plot using matplotlib and pyplot libraries and in a heatmap using seaborn library.
5. Features were retrieved from the DataFrame which includes all the columns except ‘status’.
6. Labels were retrieved from the DataFrame which is the ‘status’ column. (Reference 4)
7. Features were scaled between -1 and 1.
8. The data set was split (80-20) between train and test.
9. A Decision Tree Classifier model was fitted with the train data and accuracy was checked on the test set.
10. A Random Forest Classifier model was fitted with the train data and accuracy was checked on the test set.
11. An XGBoost Classifier model was fitted with the trained data, hyperparameters were tuned. 
12. Confusion matrix and classification reports were generated to check accuracy and precision on the test set.

__Results:__

In this study, the training dataset was fitted with three different types of Classification Algorithms; Decision Tree, Random Forest, and XGBoost and their accuracy were checked on the testing dataset and the results are as follows: 

1. Accuracy of Decision Tree Classifier Model: 89.7 %
2. Accuracy of Random Forest Classifier Model: 97.4 %
3. Accuracy of XGBoost Classifier Model: 100.0 %

![](https://github.com/SKandar-1/Figures/blob/main/XGBoost_Parkinsons_Confusion_Matrix.png)

__Figure 1:__ Confusion Matrix for the XGBoost Classification Model.
![](https://github.com/SKandar-1/Figures/blob/main/XGBoost_Parkinsons_Classification_Report.PNG)

__Figure 2:__ Classification Report for the XGBoost Model.

__Conclusions:__

As expected, the accuracy of the models gradually increased from Decision Tree to Random Forest to XGBoost Classifier algorithms and the XGBoost model was able to predict Parkinson's disease with 100% accuracy on the testing dataset, i.e., no false positive or false negative result was predicted.


__References:__
1. https://parkinsonfoundation.org/
2. 'Exploiting Nonlinear Recurrence and Fractal Scaling Properties for Voice Disorder Detection', Little MA, McSharry PE, Roberts SJ, Costello DAE, Moroz IM. BioMedical Engineering OnLine 2007, 6:23 (26 June 2007)
3. https://archive.ics.uci.edu/ml/machine-learning-databases/parkinsons/
4. https://data-flair.training/blogs/python-machine-learning-project-detecting-parkinson-disease/

