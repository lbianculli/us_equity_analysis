
This repository will walk through a holistic process of preprocessing and premodeling data in preparation for feeding a machine learning algorithm. After premodeling, various models are explored, the best of which is thoroughly evaluated.

# Topics
  1. Preprocessing: Perform fundamental data preprocessing starting with previously-scraped US pricing, macro, and fundamental data. This short notebook walks through how to deal with missing values, handling outliers, scaling data, and augmenting data with additional metrics based on data collected from financial statements.

  2. Premodeling: A longer notebook in which many of the steps may also be classified as preprocessing. The focus of this code is to specifically prepare our data for feeding through a Machine Learning model in Python. This notebook contains 500-1000 lines of code focused on: examining and visualizaing linear interactions, measuring feature importance, and reducing our feature space.

  3. Model Selection: Split data into train, test, and holdout data and use SKLearn's GridSearch class to determine the best model and perform hyperparameter tuning.

  4. Model Evaluation: With the fully trained model and holdout data available, this notebook starts by confirming efficiacy of the model on the holdout data, after which the performance of the model is analyzed according to various metrics such as F1 score, confusion matrix, and the ROC/AUC score. Finally, using optimal thresholds determined by the ROC/AUC curve, securities that would have been chosen by the model in a prior period are measured and evaluated against returns of the S&P500 ETF during the same time period.
  
