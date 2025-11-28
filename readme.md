# 💳 Credit Application Prediction – Machine Learning Project
This project was created to predict whether an individual's credit application would be approved or not.  
The dataset contains anonymized information about applicants in Germany and was analyzed using classification algorithms.

## 🎯 Project Goal
Banks evaluate the risk of an applicant when granting credit.  
In this project, we attempted to predict whether an application would be approved based on some provided financial and personal information.

## 📁 Dataset Used
**Source:** UCI German Credit Data  
**Total Observations:** 1000  
**Target Variable:** Credit Approval (1 = Approved, 0 = Rejected)

## 🔧 Steps Taken
- Explored the data and transformed categorical variables appropriately (using `get_dummies`).  
- Split the data into training and test sets (80% / 20%).  
- Applied standardization for KNN and SVM (using `StandardScaler`).  
- Tested 3 different classification algorithms:  
  - Random Forest ✅  
  - K-Nearest Neighbors  
  - Support Vector Machine  

## 📊 Results
The best performance was achieved with Random Forest, reaching an accuracy of approximately 79.5%.

| Model          | Accuracy |
|----------------|---------|
| Random Forest  | 79.5% ✅ |
| KNN            | 75.0%   |
| SVM            | 78.0%   |

We also observed which features the model focused on the most using a feature importance graph.

## 🧪 Libraries Used
- `pandas`, `numpy`  
- `scikit-learn` (for modeling and evaluation)  
- `matplotlib`, `seaborn` (for visualization)

## 📌 File Structure
```text
kredi-basvuru-tahmin/
├── main.ipynb             # Model creation notebook
├── german_credit_data.csv
├── classification_report.txt
├── random_forest_model.pkl # Saved trained model
└── README.md               # Project description
```

## 🙋🏻‍♂️ Why I Did This Project
I wanted to experiment with classification models on a real dataset as part of my data science journey.  
I thought that a topic like credit applications is important both in business and technically.  
Throughout the project, I better understood how to improve model performance and how critical data preprocessing is.

## 👨‍💻 Author
Zeynep Şura Kaya  
Computer Engineering


