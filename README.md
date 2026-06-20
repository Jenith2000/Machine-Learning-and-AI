# BBIM708 - Machine Learning & AI Portfolio

# Overview

This project was completed for the BBIM708 / GDDA708 Machine Learning and AI course at New Zealand Skills and Education College (NZSE).

The objective was to evaluate machine learning algorithms on real-world datasets and improve their performance using hyperparameter tuning techniques such as Grid Search, Random Search, and 5-Fold Cross-Validation.

# Learning Outcomes

- Part A : Evaluate machine learning algorithms for AI applications.
- Part B : Apply fine-tuning methods to optimize machine learning model performance.

# Datasets

Breast Cancer Wisconsin Dataset ('Grid search.csv')

- Task: Classification
- Records: 569
- Features: 30 numerical measurements
- Target: Diagnosis (Malignant or Benign)

Ames Housing Dataset ('Random search.csv')

- Task: Regression
- Records: 1,460
- Features: 79 housing-related attributes
- Target: SalePrice

Mall Customer Segmentation Dataset ('unsupervised.csv')

- Task: Clustering
- Records: 200
- Features:

  * CustomerID
  * Gender
  * Age
  * Annual Income
  * Spending Score

# Algorithms Used

## Part A - Supervised Learning

### Random Forest Classifier

- Type: Supervised Learning
- Purpose: Predict breast cancer diagnosis (Malignant or Benign)

### Logistic Regression

- Type: Supervised Learning
- Purpose: Binary classification with probability output

## Part A - Unsupervised Learning

### K-Means Clustering

- Type: Unsupervised Learning
- Purpose: Identify natural customer segments using the Elbow Method

### Hierarchical Clustering

- Type: Unsupervised Learning
- Purpose: Discover customer segments using a dendrogram structure

## Part B - Fine-Tuning Techniques

### Grid Search + Random Forest Classifier

- Optimize classification hyperparameters
- Parameters tuned:

  * n_estimators
  * max_depth

### Random Search + Random Forest Regressor

- Optimize regression hyperparameters
- Parameters tuned:

  * n_estimators
  * max_depth

### 5-Fold Cross-Validation

- Evaluate model reliability
- Assess model generalization performance

# Results

## Classification Results (Breast Cancer Dataset)

### Random Forest Classifier

- Accuracy: 97.37%
- Precision: 100.00%
- Recall: 92.86%
- F1-Score: 96.30%
- ROC-AUC: 99.29%

### Logistic Regression

- Accuracy: 96.49%
- Precision: 97.50%
- Recall: 92.86%
- F1-Score: 95.12%
- ROC-AUC: 99.60%

## Clustering Results (Mall Customer Dataset)

### K-Means Clustering

- Number of Clusters (k): 5
- Silhouette Score: 0.5547
- Inertia (WCSS): 65.57
- Cluster Selection Method: Elbow Method

### Hierarchical Clustering (Ward)

- Number of Clusters (k): 5
- Silhouette Score: 0.5538
- Linkage Method: Ward
- Cluster Selection Method: Dendrogram

## Grid Search Optimization

### Random Forest Classifier

#### Before Tuning (Decision Tree Baseline)

- Accuracy: 92.98%
- F1-Score: 90.48%

#### After Tuning (Random Forest + Grid Search)

- Accuracy: 97.37%
- F1-Score: 96.30%

#### Best Parameters

python :
n_estimators = 50 , 
max_depth = None

## Random Search Optimization

### Random Forest Regressor

#### Before Tuning (Decision Tree Baseline)

- RMSE: $42,097
- MAE: $27,759
- R²: 0.7690

#### After Tuning (Random Forest Regressor + Random Search)

- RMSE: $28,865
- MAE: $17,637
- R²: 0.8914

#### Best Parameters

python : 
n_estimators = 269 , 
max_depth = 12

## 5-Fold Cross-Validation Results

### Random Forest Classifier

- Mean Accuracy: 95.96%
- Mean F1-Score: 94.52%

### Random Forest Regressor

- Mean RMSE: $30,572
- Mean R²: 0.8352

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- SciPy

## Installation

Install the required Python libraries:

bash : 
pip install pandas numpy matplotlib seaborn scikit-learn scipy gdown

# How to Run This Code

Option 1 — Open directly in Google Colab

Step-by-step instructions:

Step 1 — Open Google Colab
Go to colab.research.google.com and sign in with a Google account.

Step 2 — Open the notebook from GitHub


Click File in the top menu
Click Open notebook
Click the GitHub tab
Type in this repository URL:

  https://github.com/Jenith2000/Machine-Learning-and-AI

Click the search icon
Click on Assessment_ML.ipynb from the list that appears

Step 3 — Run all cells


Click Runtime in the top menu
Click Run all
Wait for all cells to finish running (this takes about 2–3 minutes)
All outputs, charts and results will appear below each cell


Step 4 — View the results
All figures, tables and printed results will appear directly below their code cells in the notebook.


# Option 2 — Run locally using VS Code

Step 1 — Download the repository


Go to the repository page on GitHub
Click the green Code button
Click Download ZIP
Extract the ZIP file to a folder on your computer


Step 2 — Install Python
Download and install Python 3.11 or newer from python.org

Step 3 — Install VS Code
Download from code.visualstudio.com and install it.

Step 4 — Install the Jupyter extension in VS Code


Open VS Code
Click the Extensions icon on the left sidebar
Search for Jupyter and click Install
Search for Python and click Install


Step 5 — Install required libraries
Open the VS Code terminal (press Ctrl + `) and run:

bash : pip install pandas numpy matplotlib seaborn scikit-learn scipy gdown

Step 6 — Open the notebook


In VS Code click File → Open Folder
Select the folder where you extracted the ZIP
Click on Assessment_ML.ipynb in the file explorer on the left


Step 7 — Run the notebook

Press Ctrl + Shift + P
Type Run All and press Enter
All cells will run from top to bottom

