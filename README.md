# Credit Card Fraud Detection Using Machine Learning

## 📌 Project Overview

Credit Card Fraud Detection is a Machine Learning project that identifies potentially fraudulent credit card transactions using a **Random Forest Classifier**. The model analyzes transaction data, classifies transactions as genuine or fraudulent, and evaluates its performance using various classification metrics.

## 🎯 Objectives

- Analyze credit card transaction data.
- Identify fraudulent and genuine transactions.
- Train a Machine Learning classification model.
- Evaluate model performance using classification metrics.
- Visualize the confusion matrix, ROC curve, and feature importance.
- Identify detected and missed fraudulent transactions.

## 🛠️ Technologies Used

- **Programming Language:** Python
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn
- **Machine Learning:** Scikit-learn
- **Development Environment:** Jupyter Notebook / Google Colab

## 📂 Dataset

The project uses a credit card transaction dataset named `creditcard.csv`.

The target column is `Class`, which represents the transaction type:

- `0` – Genuine transaction
- `1` – Fraudulent transaction

**Note:** The dataset is not included in this repository. Download the dataset separately and update the file path in the notebook according to your environment.

## ⚙️ Project Workflow

1. **Data Loading:** Load the dataset using Pandas.
2. **Data Exploration:** Examine the dataset structure, data types, missing values, and class distribution.
3. **Data Preparation:** Separate the input features and target variable.
4. **Data Splitting:** Split the dataset into 80% training data and 20% testing data.
5. **Model Training:** Train a Random Forest Classifier with 100 decision trees.
6. **Prediction:** Predict whether transactions are genuine or fraudulent.
7. **Model Evaluation:** Evaluate performance using precision, recall, F1-score, ROC-AUC, and the classification report.
8. **Fraud Analysis:** Analyze detected and missed fraudulent transactions.
9. **Feature Importance:** Identify and visualize the ten most important features.
10. **Visualization:** Generate the confusion matrix and ROC curve.

## 🤖 Machine Learning Algorithm

### Random Forest Classifier

Random Forest is a supervised Machine Learning algorithm that combines multiple decision trees to make predictions. In this project, it is used to classify credit card transactions as genuine or fraudulent.

**Model Configuration:**

- **Number of Estimators:** 100
- **Class Weight:** `balanced_subsample`
- **Random State:** 42
- **Test Size:** 20%
- **Parallel Processing:** `n_jobs=-1`

## 📊 Evaluation Metrics

The model's performance is evaluated using the following metrics:

- **Precision:** Measures how many transactions predicted as fraudulent are actually fraudulent.
- **Recall:** Measures how many actual fraudulent transactions are correctly detected.
- **F1-Score:** Provides a balance between precision and recall.
- **ROC-AUC:** Measures the model's ability to distinguish between genuine and fraudulent transactions.
- **Confusion Matrix:** Displays the number of correct and incorrect predictions for each class.
- **Classification Report:** Provides precision, recall, F1-score, and support for each class.

## 📈 Project Outputs

After executing the notebook, the following outputs are generated:

- Confusion matrix visualization.
- Classification report and evaluation metrics.
- Counts of detected and missed fraudulent transactions.
- Top 10 feature importance visualization.
- ROC curve visualization.
- `actual_fraudulent_test_transactions.csv` containing actual fraudulent transactions from the test dataset.

## 🔮 Future Enhancements

- Compare Random Forest with other Machine Learning algorithms.
- Perform hyperparameter tuning to improve model performance.
- Apply cross-validation for more reliable evaluation.
- Optimize the prediction threshold to balance fraud detection and false alarms.
- Develop a web application for real-time fraud prediction.

## ⚠️ Limitations

- Fraudulent transactions are much less common than genuine transactions, resulting in an imbalanced dataset.
- Accuracy alone may not provide a reliable measure of fraud detection performance.
- Model performance depends on the dataset quality, selected features, and model configuration.
- The project is intended for educational purposes and is not a production-ready fraud prevention system.
