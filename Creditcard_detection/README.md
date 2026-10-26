Credit Card Fraud Detection Using Random Forest
📌 Project Overview
This project implements a Machine Learning model for detecting fraudulent credit card transactions using the Random Forest Classifier.

The project covers the complete machine learning workflow:

Loading the dataset
Exploring the data
Checking missing values
Analyzing class distribution
Preparing features and target variables
Handling missing values
Splitting the dataset into training and testing sets
Training a Random Forest model
Making predictions
Evaluating model performance
Visualizing the confusion matrix
Identifying important features
📊 Dataset
The project uses the creditcard.csv dataset.

The dataset contains:

5,974 rows
31 columns
30 input features
1 target variable (Class)
The target variable Class represents:

Class	Meaning
0	Genuine transaction
1	Fraudulent transaction
The dataset contains 13 missing values.

Class Distribution
The dataset is highly imbalanced:

Genuine transactions: 5,970
Fraudulent transactions: 3
Genuine: 99.9498%
Fraud: 0.0502%
🧾 Features
The model uses the following 30 features:

Time
V1
V2
V3
V4
V5
V6
V7
V8
V9
V10
V11
V12
V13
V14
V15
V16
V17
V18
V19
V20
V21
V22
V23
V24
V25
V26
V27
V28
Amount
The Class column is used as the target variable.

🛠️ Technologies Used
Python
Pandas
NumPy
Matplotlib
Seaborn
Scikit-learn
Google Colab / Jupyter Notebook
🔄 Machine Learning Workflow
1. Import Libraries
The project uses Pandas, NumPy, Seaborn, Matplotlib, and Scikit-learn libraries.

2. Load Dataset
The dataset is loaded using:

df = pd.read_csv("/content/creditcard.csv")
The notebook then displays the dataset shape, first few records, data information, missing values, and class distribution.

3. Data Preprocessing
Missing rows are removed using:

df_clean = df.dropna()
The features and target are then separated:

X_clean = df_clean.drop("Class", axis=1)
y_clean = df_clean["Class"]
The data is divided into training and testing sets using an 80/20 split, with stratification and random_state=42.

4. Train/Test Split
The resulting datasets contain:

Dataset	Shape
Training data	(4778, 30)
Testing data	(1195, 30)
5. Model Training
A Random Forest Classifier is used:

RandomForestClassifier(
    n_estimators=100,
    class_weight="balanced_subsample",
    random_state=42,
    n_jobs=-1
)
The model is trained using the training dataset.

6. Prediction
The trained model generates:

Predicted transaction classes
Fraud probabilities
y_pred = model.predict(X_test)
y_prob = model.predict_proba(X_test)[:, 1]
📈 Model Evaluation
The model is evaluated using:

Confusion Matrix
Precision
Recall
F1-score
ROC-AUC
Classification Report
The notebook generates the confusion matrix with Genuine and Fraud labels.

Confusion Matrix
The resulting confusion matrix is:

[[1194    0]
 [   1    0]]
This means that the test set contained 1 fraudulent transaction, which the model classified as genuine.

⚠️ Important Observation
The dataset is extremely imbalanced, containing only 3 fraudulent transactions out of 5,974 records.

Because there is only one fraud case in the test set, metrics such as recall, precision, and F1-score should be interpreted carefully.

A high ROC-AUC alone does not necessarily mean that the model is effective at detecting actual fraudulent transactions.

📁 Project Structure
Credit-Card-Fraud-Detection/
│
├── Task7_ML(1).ipynb
├── creditcard.csv
└── README.md
▶️ How to Run
Step 1: Install Required Libraries
pip install pandas numpy seaborn matplotlib scikit-learn
Step 2: Add the Dataset
Place the dataset in the required location:

/content/creditcard.csv
Step 3: Open the Notebook
Open:

Task7_ML(1).ipynb
in Google Colab or Jupyter Notebook.

Step 4: Run the Notebook
Run all cells sequentially to:

Load the dataset
Explore the data
Handle missing values
Split the dataset
Train the Random Forest model
Generate predictions
Evaluate the model
Display the confusion matrix
🎯 Conclusion
This project demonstrates how a Random Forest Classifier can be applied to credit card fraud detection.

The project also highlights an important challenge in fraud detection: severe class imbalance. Since fraudulent transactions are extremely rare compared with genuine transactions, model evaluation should focus carefully on fraud-specific metrics such as precision, recall, and F1-score, rather than relying only on overall performance measures.

👩‍💻 Project
Machine Learning – Credit Card Fraud Detection

Built using Python and Scikit-learn.
