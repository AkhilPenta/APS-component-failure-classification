# APS-component-failure-classification
This is an end to end case study on APS component failure classification in Scania Trucks

Dataset: [APS Failure at Scania Trucks Data Set](https://archive.ics.uci.edu/ml/datasets/APS+Failure+at+Scania+Trucks)

## Contents:

### [EDA & Preprocessing.ipynb](https://github.com/AkhilPenta/APS-component-failure-classification/blob/main/EDA%20%26%20Preprocessing.ipynb)
  ### 1. Business Problem
      1.1. Description
      1.2 Sources/Useful Links
      1.3 Real world/Business Objectives and Constraints
  ### 2. Machine Learning Probelm
      2.1 Data
        2.1.1 Data Overview
        2.1.2 Example Data point
      2.2 Mapping the real world problem to an ML problem
        2.2.1 Type of Machine Leaning Problem
        2.2.2 Performance Metric
      2.3 Train and Test Construction
  ### 3. Exploratory data analysiss
      3.1 Train Data
      3.2 Test Data
  ### 4. Preprocessing Data
      4.1 Train Data
      4.2 Test Data
      4.3 Standardization
      4.4 Handling Missing Data - Imputation
        4.4.1 Median Imputer
        4.4.2 KNNImputer
        4.4.3 IterativeImputer with BayesianRidge regressor
        4.4.4 Imputation based on Regression model - RandomForestRegressor
        4.4.5 Imputaion based on BayesianGaussianMixture model
      4.5 Quality Check of above Impuation Methods
      4.6 Missing Indicator - Feature generation
      
### [ML Models - 1.ipynb](https://github.com/AkhilPenta/APS-component-failure-classification/blob/main/ML%20Models%20-%201.ipynb)    
  ### 5. Machine Learning Models - 1
      5.1 Utility Functions
        5.1.1 Upsampling function
        5.1.2 utility function for Hyperparameter tuning and for extracting & saving result values
        5.1.3 Functions for implementing MetaLearnClassifier
        5.1.4 utility function for MetaLearnClassifier: Hyperparameter tuning, Computing and reporting scores of classifier model
      5.2 Median Imputed Dataset
        5.2.1 loading Train, CV & Test datasets & Upsampling train dataset
        5.2.2 LogisticRegression on Median Imputed Data
        5.2.3 LinearSVC on Median Imputed Data
        5.2.4 RandomForestClassifier on Median Imputed Data
        5.2.5 XGBClassifier on Median Imputed Data
        5.2.6 AdaBoostClassifier on Median Imputed Data
        5.2.7 MetaLearnClassifier on Median Imputed Data
      5.3 KNNImputer Imputed Dataset
        5.3.1 loading Train, CV & Test datasets & Upsampling train dataset
        5.3.2 LogisticRegression on KNNImputer Imputed Data
        5.3.3 LinearSVC on KNNImputer Imputed Data
        5.3.4 RandomForestClassifier on KNNImputer Imputed Data
        5.3.5 XGBClassifier on KNNImputer Imputed Data
        5.3.6 AdaBoostClassifier on KNNImputer Imputed Data
        5.3.7 MetaLearnClassifier on KNNImputer Imputed Data
      5.4 BayesianRidge_imputer Imputed Dataset
        5.4.1 loading Train, CV & Test datasets & Upsampling train dataset
        5.4.2 LogisticRegression on BayesianRidge_imputer Imputed Data
        5.4.3 LinearSVC on BayesianRidge_imputer Imputed Data
        5.4.4 RandomForestClassifier on BayesianRidge_imputer Imputed Data
        5.4.5 XGBClassifier on BayesianRidge_imputer Imputed Data
        5.4.6 AdaBoostClassifier on BayesianRidge_imputer Imputed Data
        5.4.7 MetaLearnClassifier on BayesianRidge_imputer Imputed Data
      5.5 RandomForestRegressor_imputer Imputed Dataset
        5.5.1 loading Train, CV & Test datasets & Upsampling train dataset
        5.5.2 LogisticRegression on RandomForestRegressor_imputer Imputed Data
        5.5.3 LinearSVC on RandomForestRegressor_imputer Imputed Data
        5.5.4 RandomForestClassifier on RandomForestRegressor_imputer Imputed Data
        5.5.5 XGBClassifier on RandomForestRegressor_imputer Imputed Data
        5.5.6 AdaBoostClassifier on RandomForestRegressor_imputer Imputed Data
        5.5.7 MetaLearnClassifier on RandomForestRegressor_imputer Imputed Data
      5.6 BayesianGaussianMixture_imputer Imputed Dataset
        5.6.1 loading Train, CV & Test datasets & Upsampling train dataset
        5.6.2 LogisticRegression on BayesianGaussianMixture_imputer Imputed Data
        5.6.3 LinearSVC on BayesianGaussianMixture_imputer Imputed Data
        5.6.4 RandomForestClassifier on BayesianGaussianMixture_imputer Imputed Data
        5.6.5 XGBClassifier on BayesianGaussianMixture_imputer Imputed Data
        5.6.6 AdaBoostClassifier on BayesianGaussianMixture_imputer Imputed Data
        5.6.7 MetaLearnClassifier on BayesianGaussianMixture_imputer Imputed Data
  ### 6 Results & Summary - 1
        
### [ML Models - 2.ipynb](https://github.com/AkhilPenta/APS-component-failure-classification/blob/main/ML%20Models%20-%202.ipynb)
  ### 7. Machine Learning Models - 2
      7.1 Utility Functions
        7.1.1 Upsampling function
        7.1.2 utility function for Hyperparameter tuning and for extracting & saving result values
      7.2 Median Imputed + Missing Indicator Dataset
        7.2.1 loading Train, CV & Test datasets & Upsampling train dataset
        7.2.2 RandomForestClassifier on Median Imputed + Missing Indicator Data
        7.2.3 XGBClassifier on Median Imputed + Missing Indicator Data
      7.3 KNNImputer Imputed + Missing Indicator Dataset
        7.3.1 loading Train, CV & Test datasets & Upsampling train dataset
        7.3.2 RandomForestClassifier on KNNImputer Imputed + Missing Indicator Data
        7.3.3 XGBClassifier on KNNImputer Imputed + Missing Indicator Data
      7.4 BayesianRidge_imputer Imputed + Missing Indicator Dataset
        7.4.1 loading Train, CV & Test datasets & Upsampling train dataset
        7.4.2 RandomForestClassifier on BayesianRidge_imputer Imputed + Missing Indicator Dat
        7.4.3 XGBClassifier on BayesianRidge_imputer Imputed + Missing Indicator Data
      7.5 RandomForestRegressor_imputer Imputed + Missing Indicator Dataset
        7.5.1 loading Train, CV & Test datasets & Upsampling train dataset
        7.5.2 RandomForestClassifier on RandomForestRegressor_imputer Imputed + Missing Indicator Data
        7.5.3 XGBClassifier on RandomForestRegressor_imputer Imputed + Missing Indicator Dat
      7.6 BayesianGaussianMixture_imputer Imputed + Missing Indicator Dataset
        7.6.1 loading Train, CV & Test datasets & Upsampling train dataset
        7.6.2 RandomForestClassifier on BayesianGaussianMixture_imputer Imputed + Missing Indicator Data
        7.6.3 XGBClassifier on BayesianGaussianMixture_imputer Imputed + Missing Indicator Data
  ### 8 Results & Summary - 2
  
### [Final.ipynb](https://github.com/AkhilPenta/APS-component-failure-classification/blob/main/Final.ipynb)
  ### 9 Final Functions
      9.1 Final Function - 1
      9.2 Final Function - 2
      
  
