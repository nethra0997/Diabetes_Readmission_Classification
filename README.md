# Diabetes_Readmission_Classification
# Project Title: Classification for Early Readmission of Diabetic Patients

Objective: The primary goal of this project was to develop a predictive model to classify whether diabetic patients would be readmitted to the hospital within 30 days of discharge. This involved extensive data cleaning, preprocessing, visualization, and model building to improve patient care and reduce healthcare costs.


Dataset: UCI Diabetes Dataset
Duration: 1999-2008
Records: 101,766 patient encounters
Features: 47 features including demographic information, diagnostic data, and treatment details

# Key Steps:

# Data Cleaning and Preprocessing:
Replaced missing and invalid values
Dropped columns with significant missing data
Removed redundant or invariant features
Merged similar categories for certain features
Encoded categorical variables using binary and one-hot encoding
Transformed age ranges to numerical midpoints
Created new feature columns for diagnosis categories
Ensured data integrity by removing duplicate entries

# Exploratory Data Analysis (EDA):
Conducted univariate and bivariate analysis to understand the data distribution
Visualized numerical and categorical variables using box plots, distribution plots, count plots, and correlation heatmaps

# Feature Engineering:
Applied Principal Component Analysis (PCA) to reduce dimensionality and retain essential information
Focused on simplifying the dataset for better model performance

# Model Building and Evaluation:
Logistic Regression: Baseline model for binary classification
Neural Networks: Modelled complex, non-linear relationships in the data using Keras
K-Nearest Neighbors (K-NN): Classified data points based on similarity using Euclidean distance
Employed K-Fold Cross-Validation to ensure model robustness and mitigate overfitting
Evaluated models using metrics such as accuracy, precision, recall, F1 score, and ROC curves

# Results:
Logistic Regression: Accuracy of 44.8%, Recall of 65.15%, Precision of 10.07%, F1 score of 17.44%
Neural Network: Accuracy of 50.07%, Recall of 100%, indicating a bias towards predicting one class
K-NN: Accuracy of 90.46% with k=2, but low precision and recall due to the accuracy paradox
Improved model performance post-PCA for Logistic Regression and Neural Network

# Conclusion:
The Neural Network model with PCA showed the best performance, achieving a balanced accuracy, precision, recall, and a low cost value. It demonstrated the effectiveness of dimensionality reduction in enhancing model performance for complex datasets.
The project underscored the potential of machine learning in healthcare, particularly in predicting patient readmissions and improving care management.

# Tech Stack:
Programming Languages: Python
Libraries: Keras, Scikit-learn, Pandas, NumPy, Matplotlib
Techniques: Logistic Regression, Neural Networks, K-Nearest Neighbors, K-Fold Cross-Validation, Principal Component Analysis (PCA)
Tools: Jupyter Notebook for coding and analysis
