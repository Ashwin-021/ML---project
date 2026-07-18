# Student Placement Prediction using Machine Learning

## 📌 Project Overview
This project predicts whether a student will be placed or not placed based on academic and activity-based details.  
It uses Machine Learning to analyze student performance and predict placement status.

## 🎯 Objective
The main objective of this project is to build a simple Machine Learning model that predicts student placement using factors like study hours, attendance, previous score, exam score, sleep hours, internet usage, and assignments completed.

## 📂 Dataset
The dataset contains 10,000 student records.

### Features Used
- study_hours
- attendance
- sleep_hours
- internet_usage
- assignments_completed
- previous_score
- exam_score

### Target Column
- placement_status

## 🛠️ Technologies Used
- Python
- Pandas
- Matplotlib
- Seaborn
- Scikit-Learn
- Google Colab
- Logistic Regression

## 🔄 Project Workflow
1. Import required libraries
2. Load the student dataset
3. Display dataset using `head()`
4. Check dataset information using `info()`
5. Check missing values
6. Visualize placement distribution
7. Select input and output columns
8. Split data into training and testing data
9. Apply StandardScaler
10. Train Logistic Regression model
11. Predict placement status
12. Check model accuracy
13. Test with new student data

## 📊 Visualizations
This project includes:
- Placement status count plot
- Study hours vs placement status
- Attendance vs placement status
- Exam score vs placement status
- Confusion matrix

## 🤖 Machine Learning Model
The model used in this project is:

### Logistic Regression
Logistic Regression is used because this is a classification problem.  
The output is either:

- Placed
- Not Placed

## ✅ Output
The model predicts whether a student is:

```text
Placed
Not Placed

