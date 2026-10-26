# 💳 Credit Card Fraud Detection Using Machine Learning

## 📌 Project Overview

This Machine Learning project detects fraudulent credit card transactions using the **Random Forest Classifier**. The model analyzes transaction details and predicts whether a transaction is genuine or fraudulent.

The main goal of this project is to identify suspicious transactions, reduce financial losses, and help improve fraud detection systems.

## 🎯 Problem Statement

Credit card fraud is a major challenge in the financial industry. Detecting fraudulent transactions accurately is important for protecting customers and financial institutions.

This project uses Machine Learning to classify transactions into two categories:

* **Class 0:** Genuine transaction
* **Class 1:** Fraudulent transaction

## 🎯 Objectives

* Analyze credit card transaction data.
* Identify missing values and examine class distribution.
* Prepare the dataset for Machine Learning.
* Train a Random Forest classification model.
* Predict fraudulent transactions.
* Evaluate model performance using classification metrics.
* Identify important features influencing predictions.

## 📂 Project Structure

```text
Credit-Card-Fraud-Detection/
│
├── Dataset/
│   └── creditcard.csv
│
├── Notebook/
│   └── Creditcard_Notebook.ipynb
│
├── Output/
│   ├── Confusion_Matrix.png
│   ├── ROC_Curve.png
│   └── Feature_Importance.png
│
├── actual_fraudulent_test_transactions.csv
└── README.md
```

*Note: Save the generated graphs in the `Output` folder if you want to include them in your GitHub repository. The fraud transaction CSV is generated when the notebook runs.*

## 📊 Dataset Description

The dataset contains credit card transaction records with features describing transaction information.

Important columns include:

* **Time:** Time elapsed between transactions, as represented in the dataset.
* **Amount:** Transaction amount.
* **V1–V28:** Anonymized numerical features.
* **Class:** Target variable indicating whether the transaction is genuine or fraudulent.

### Target Variable

| Class | Description            |
| ----- | ---------------------- |
| 0     | Genuine transaction    |
| 1     | Fraudulent transaction |

The dataset typically contains a highly imbalanced class distribution, with fraudulent transactions representing a small proportion of all transactions.

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Jupyter Notebook / Google Colab

## ⚙️ Project Workflow

### 1. Data Loading

Load the credit card dataset using Pandas and examine the first few records and dataset dimensions.

### 2. Data Exploration

* Inspect dataset information and column names.
* Check for missing values.
* Analyze the distribution of genuine and fraudulent transactions.
* Calculate the class percentages.

### 3. Data Preprocessing

* Remove rows containing missing values.
* Separate the input features from the target variable.
* Split the dataset into training and testing sets.
* Use stratified splitting to preserve the class distribution.

### 4. Model Training

Train a Random Forest Classifier with the following configuration:

* Number of estimators: 100
* Class weighting: `balanced_subsample`
* Random state: 42
* Parallel processing: Enabled

Class weighting helps the model account for the imbalance between genuine and fraudulent transactions.

### 5. Fraud Prediction

The trained model predicts the transaction class and calculates the probability of fraud for each test transaction.

### 6. Model Evaluation

Evaluate the model using:

* **Confusion Matrix:** Shows correct and incorrect predictions.
* **Precision:** Measures how many transactions predicted as fraudulent are actually fraudulent.
* **Recall:** Measures how many actual fraudulent transactions are detected.
* **F1-Score:** Balances precision and recall.
* **ROC-AUC Score:** Measures how well the model distinguishes between genuine and fraudulent transactions.
* **Classification Report:** Provides precision, recall, F1-score, and support for each class.

### 7. Feature Importance

Identify the top 10 important features used by the Random Forest model and visualize their relative importance.

### 8. Fraud Transaction Analysis

* Extract actual fraudulent transactions from the test dataset.
* Identify detected and missed fraud cases.
* Save the actual fraudulent test transactions to a CSV file.

## 📈 Visualizations

The notebook generates the following visualizations:

1. **Confusion Matrix:** Displays the classification results for genuine and fraudulent transactions.
2. **ROC Curve:** Illustrates the model's ability to distinguish between the two classes across different thresholds.
3. **Feature Importance Chart:** Displays the 10 most important input features.

These visualizations help interpret model performance and understand the factors contributing to fraud predictions.

## ▶️ How to Run the Project

### Step 1: Clone the Repository

```bash
git clone <your-repository-url>
cd Credit-Card-Fraud-Detection
```

### Step 2: Install the Required Libraries

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

### Step 3: Place the Dataset

Download `creditcard.csv` and place it in the appropriate folder.

### Step 4: Open the Notebook

Open `Creditcard_Notebook.ipynb` in Jupyter Notebook or Google Colab.

### Step 5: Update the Dataset Path

The notebook currently uses a Google Colab path:

```python
df = pd.read_csv("/content/creditcard.csv")
```

For a local project, update the path according to your folder structure. For example:

```python
df = pd.read_csv("Dataset/creditcard.csv")
```

### Step 6: Run All Cells

Execute the notebook cells in order to preprocess the data, train the model, evaluate its performance, and generate the visualizations and fraud transaction report.

## 📋 Expected Output

After running the notebook, the project produces:

* Dataset information and class distribution.
* Training and testing data.
* Predicted transaction classes and fraud probabilities.
* Confusion matrix and classification report.
* Precision, recall, F1-score, and ROC-AUC score.
* Top 10 important features.
* ROC curve visualization.
* CSV file containing actual fraudulent transactions from the test set.

*Actual evaluation scores depend on the dataset and model execution. Run the notebook to obtain the results.*

## 🚀 Future Improvements

* Experiment with other classification algorithms.
* Apply additional techniques for imbalanced datasets, such as SMOTE.
* Tune model hyperparameters to improve performance.
* Compare models using precision, recall, F1-score, and ROC-AUC.
* Develop a web application for real-time fraud prediction.
* Explore deployment options for integrating fraud detection into financial systems.

## ⚠️ Limitations

* The dataset may contain highly imbalanced classes.
* Anonymized features can make the results difficult to interpret.
* Model predictions are not guaranteed to identify every fraudulent transaction.
* The model requires further testing before use in real financial systems.

## 👨‍💻 Conclusion

This project demonstrates how Machine Learning can be applied to credit card fraud detection using a Random Forest Classifier. It includes data exploration, preprocessing, model training, fraud prediction, performance evaluation, and feature importance analysis.

The project provides practical experience with Python, Pandas, data analysis, classification algorithms, and model evaluation.

---

**Project Type:** Machine Learning – Classification

**Algorithm:** Random Forest Classifier

**Language:** Python
