# Data-Analytics-on-Diabetes-Dataset


## Description
-----------------
The proposed framework for this project is shown in the figure below. The proposed framework is inspired by the existing studies related to the study of microbiome data with the utilisation of machine learning (Bakir-Gungor et al., 2021, 2022). The framework is started with data pre-processing followed by supervised and unsupervised learning. The data pre-processing part includes the combination of the healthy and diabetes dataset, removing the duplication of the combined dataset, SMOTE analysis to ensure that the dataset is balanced, splitting the data into training and testing sets, and the feature selection method. For supervised learning, the top 20, 50 amd 100 features from all the feature selection methods are used to train these classification models : Random Forest (RF), Adaptive Boosting (AdaBoost), Support Vector Machine (SVM), K-Nearest Neighbour (KNN), Logistic Regression (LR), Naïve Bayes (NB), Light Gradient Boosting Machine (LGBM) and Extreme Gradient Boosting (XGBoost). The models are then evaluated based on the performance metrics. K-fold cross-validation with the K value of 10 is utilised in this experiment as a source of shield against overfitting. To find out the species that are correlated to T2D, feature selection is used to identify the highly correlated features, whereas k-means clustering, and hierarchical clustering are tested to identify potential biomarkers. The data clustered are evaluated, and the output of the unsupervised learning is visualised.

![image](https://github.com/eethiing/Data-Analytics-on-Diabetes-Dataset/assets/85276977/b540c48b-3af1-4bb2-be3e-537355a80287)

## Objectives 
-----------------------
1) To find out which species of microbiota data is highly related to Type-2 Diabetes\
   Solution : Various feature selection methods are tested on the dataset as there will be over 1,000 features in the metagenome dataset. Data analysis is applied to find the features that strongly relate to T2D. The top 100 features for each selection method are extracted and the highly related species are the intersection species among of the top 100 features among few feature selection methods.
   
2) To compare the classifcation models for the diagnosis of Type 2 Diabetes\
   Solution : Metagenome dataset comes from both healthy and T2D diagnosed patients.Comparing and evaluating which classification model performs well in the diagnosis of T2D is crucial. The classification models that are being compared are : Support Vector Machine (SVM), AdaBoost, Random Forest (RF), XGBoost, K-nearest Neighbour (KNN) , Logistic Regression (LR), Naïve Bayes (NB), Light Gradient-Boosting Machine (LGBM). The models are compared based on the selected evaluation metrics.
   
3) To explore different methods to extract potential biomarkers for Type-2 Diabetes\
   Solution : To discover the potential biomarkers, unsupervised learning methods : k-means and hierarchical clustering is being used. The potential biomarkers list is obtained by getting the top 10 features of each cluster and ensuring the species exist in all clusters. The potential biomarkers that were found is being supported by literature from other studies.
   
4) To compare the execution time of the feature selection methods\
   Solution :  To find out which feature selection algorithm takes the longest time to execute. In this context, ‘time’ refers to the duration required for the feature selection algorithm to rank or identify the highly relevant features.
   

## Experimental Results
--------------------



