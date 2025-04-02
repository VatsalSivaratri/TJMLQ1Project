#   Credit Score Classification Project

This project focuses on developing robust models for classifying individuals' credit scores. The motivation is to bring more transparency and accuracy to the evaluation of credit card user trustworthiness, which is essential for a healthy relationship between banks and their customers. The goal is to use past credit card holder data to predict the likelihood of a good credit score for new customers, considering various attributes.

##   Dataset

The dataset used in this project is from a Kaggle competition. It includes a training dataset with 100,000 instances and 27 attributes. These attributes encompass both numerical data (e.g., monthly in-hand salary, outstanding debt) and categorical data (e.g., occupation, credit mix).

Key attributes include:

* Age
* Occupation
* Annual_Income
* Monthly_Inhand_Salary
* Outstanding_Debt
* Credit_Mix
* And others

The credit score is classified into three categories: Good, Poor, and Standard.

##   How to Run the Code

The main script (`Q1.ipynb`) performs several steps:

1.  **Data Loading and Preprocessing:**
    * Loads the dataset.
    * Handles missing values.
    * Cleans and transforms data (e.g., removing trailing underscores, processing age and interest rate values, converting credit history age).
    * Encodes categorical variables.
    * Handles outliers.
    * Splits the data into training and testing sets.
2.  **Model Training and Evaluation:**
    * Trains several classification models: Decision Tree, Random Forest, Logistic Regression, Naive Bayes, and SVM.
    * Evaluates the models using metrics such as accuracy, confusion matrix, True Positive Rate (TPR), False Positive Rate (FPR), and ROC-AUC.
    * Compares the performance of different models.
3.  **Feature Subset Analysis:**
    * The code also analyzes the impact of different feature subsets on model performance. It creates several data subsets based on different feature selection approaches .
    * For each subset, it trains and evaluates the same classification models.
    * The results are saved to an Excel file (`model_results_split_tpr_fpr.xlsx`) and visualized using plots.

###   Running the Main Script

To run the main analysis:

1.  Ensure that you have the required libraries installed (`numpy`, `pandas`, `scikit-learn`).
2.  Place the dataset file (`train.csv`) in the same directory as the `Q1.ipynb` file, or update the `file_path` variable in the script to point to the correct location of the dataset.
3.  Run the `Q1.ipynb` script. This will execute the data preprocessing, model training, and evaluation steps. The script will print the performance metrics for each model and generate result visualizations.