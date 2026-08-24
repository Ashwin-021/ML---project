# Customer Feedback Classifier using Machine Learning

## 📌 Project Overview

This project is a Machine Learning-based Customer Feedback Classifier that automatically predicts the category of customer feedback using Natural Language Processing (NLP). The model converts text into numerical features using TF-IDF and classifies feedback into different categories using the Multinomial Naive Bayes algorithm.

---

## 🎯 Objective

The objective of this project is to classify customer feedback into the correct category automatically, helping businesses analyze customer opinions and improve their services.

---

## 📂 Project Structure

```
Customer-Feedback-Classifier-ML/
│
├── Dataset/
│   └── customer_feedback.csv
│
├── Notebook/
│   └── Customer_Feedback_Classification.ipynb
│
├── Output/
│   ├── bar_chart.png
│   ├── pie_chart.png
│
├── requirements.txt
├── README.md
└── .gitignore
```

---

## 📊 Dataset

The dataset contains customer feedback and its corresponding category.

### Columns

- **Feedback** – Customer review or complaint
- **Category** – Category of the feedback

Example:

| Feedback | Category |
|----------|----------|
| My order has not arrived yet. | Delivery |
| The product is damaged. | Product |
| Password reset is not working. | Technical Support |

---

## 🛠️ Technologies Used

- Python
- Pandas
- Matplotlib
- Scikit-learn
- Jupyter Notebook

---

## 🤖 Machine Learning Algorithm

- TF-IDF Vectorizer
- Multinomial Naive Bayes Classifier

---

## 📈 Visualizations

The project includes:

- Feedback Category Distribution (Bar Chart)
- Feedback Category Percentage (Pie Chart)

---

## 🚀 How to Run the Project

1. Clone the repository.
2. Install the required libraries.

```bash
pip install -r requirements.txt
```

3. Open the notebook.

```
Notebook/Customer_Feedback_Classification.ipynb
```

4. Run all the cells.

---

## 📋 Output

The model predicts the category of customer feedback.

Example:

**Input**

```
I have not received my order.
```

**Prediction**

```
Delivery
```

The project also generates:

- Bar Chart
- Pie Chart

These are saved in the **Output** folder.

---

## 📌 Future Improvements

- Apply text preprocessing techniques.
- Compare multiple Machine Learning models.
- Improve prediction accuracy.
- Build a web application using Streamlit or Flask.

---

## 👨‍💻 Author

Ashwin

BCA Student | Data Science Enthusiast

