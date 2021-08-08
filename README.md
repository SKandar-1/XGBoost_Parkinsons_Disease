# XGBoost_Parkinsons_Disease

__Abstract:__

Parkinson’s Disease (PD) is a slowly progressive chronic neurologic condition which causes a gradual loss of the nerve cells in the brain. Roughly six million people worldwide suffer from Parkinson’s disease. Hyperparameter optimization was performed on the XGBoost algorithm machine learning model for the UCI ML Parkinson’s disease dataset which contains features extracted from 195 sustained vowel phonations from 31 male and female subjects, of which 23 were diagnosed with PD. This model was able to predict Parkinson's disease with 100% accuracy on the testing dataset, i.e., no false positive or false negative result was predicted.

__Introduction:__

Parkinson’s disease is second only to Alzheimer’s disease as the most prevalent neurodegenerative disease worldwide. (Reference 1) Despite extensive research, there is no known cause, cure, or prevention for Parkinson’s disease but the symptoms can be alleviated significantly with medication especially if correct diagnosis is obtained at the early stage of the disease. Little et al. from University of Oxford published a study on the Suitability of Dysphonia Measurements
for Telemonitoring of Parkinson’s Disease in 2008 where they were able achieve overall correct classification performance of 91.4%, using a kernel support vector machine. (Reference 2) In this study the default parameters for the XGBoost Classifier Model yielded an accuracy of 94% and after hyperparameter tuning the accuracy went up to 100%. 

__Methodology:__

The data file (parkinsons.data) was downloaded from UCI Machine Learning Databases. (Reference 3)
A pandas DataFrame was created from the data file.
DataFrame was checked for any duplicates and missing values.
DataFrame plotted in a scatter plot using matplotlib and pyplot libraries and in a heatmap using seaborn library.
Features were retrieved from the DataFrame which includes all the columns except ‘status’.
Labels were retrieved from the DataFrame which is the ‘status’ column. (Reference 4)
Features were scaled between -1 and 1.
The data set was split (80-20) between train and test.
A Decision Tree Classifier model was fitted with the train data and accuracy was checked on the test set.
A Random Forest Classifier model was fitted with the train data and accuracy was checked on the test set.
An XGBoost Classifier model was fitted with the trained data, hyperparameters were tuned. 
Confusion matrix and classification reports were generated to check accuracy and precision on the test set.
