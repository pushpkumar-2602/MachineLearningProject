# 🎓 Student Performance Prediction - Machine Learning Project

## 📌 Overview

This project is a Machine Learning web application built using **Flask** that predicts student performance based on various academic and demographic factors.

The model is trained using supervised learning techniques and deployed locally using Flask.

---

## 🧠 Problem Statement

To predict a student’s math score based on:

- Gender
- Race/Ethnicity
- Parental Level of Education
- Lunch Type
- Test Preparation Course
- Reading Score
- Writing Score

This helps in analyzing student performance trends and understanding key influencing factors.

---

## 🛠️ Tech Stack

- Python
- Flask
- Pandas
- NumPy
- Scikit-learn
- CatBoost
- XGBoost
- Matplotlib
- Seaborn
- Dill

---

## 📊 Machine Learning Pipeline

1. Data Collection
2. Data Preprocessing
3. Feature Engineering
4. Model Training
5. Hyperparameter Tuning
6. Model Selection
7. Model Serialization using Dill
8. Web App Integration with Flask

---

## 📂 Project Structure
src
├── __init__
├── components
│   ├── __init__
│   ├── __pycache__
│   │   ├── __init__
│   │   ├── data_ingestion
│   │   ├── data_transformation
│   │   └── model_trainer
│   ├── data_ingestion
│   ├── data_transformation
│   └── model_trainer
├── exception
├── logger
├── pipeline
│   ├── __init__
│   ├── __pycache__
│   │   ├── __init__
│   │   └── predict_pipeline
│   ├── predict_pipeline
│   └── train_pipeline
└── utils
|-- templates
|    |-- home
|    |──  index
|-- gitignore
|-- application
|-- README
|-- requirements
|-- setup

---

## 🏗️ System Architecture

```
+------------------+
|      User        |
|  (Web Browser)   |
+--------+---------+
         |
         v
+----------------------+
|   Flask Application  |
|      (app.py)        |
+--------+-------------+
         |
         v
+----------------------+
|  Data Preprocessing  |
|  (Pipeline / Utils)  |
+--------+-------------+
         |
         v
+----------------------+
|   Trained ML Model   |
|   (Saved using Dill) |
+--------+-------------+
         |
         v
+----------------------+
|  Prediction Output   |
|   (Displayed on UI)  |
+----------------------+
```

---

## 🔄 Workflow

1️⃣ User enters student details in the web form.  
2️⃣ Flask receives the input using `request.form`.  
3️⃣ Input is converted into Pandas DataFrame.  
4️⃣ Preprocessing pipeline transforms the features.  
5️⃣ Trained ML model predicts the math score.  
6️⃣ Prediction result is displayed on the webpage.

---



## 🚀 How to Run the Project Locally

### 1️⃣ Clone Repository

```
git clone https://github.com/your-username/your-repository-name.git
cd your-repository-name
```

---

### 2️⃣ Create Virtual Environment

```
python -m venv venv
```

Activate it:

Windows:
```
venv\Scripts\activate
```

Mac/Linux:
```
source venv/bin/activate
```

---

### 3️⃣ Install Requirements

```
pip install -r requirements.txt
```

---

### 4️⃣ Run Application

```
python app.py
```

Open in browser:
```
http://127.0.0.1:5000/
```

---

## 📊 Model Information

The project experiments with:

- Linear Regression  
- Random Forest  
- XGBoost  
- CatBoost  

Best performing model selected based on:

- R² Score  
- Mean Absolute Error  
- Mean Squared Error  

---

## 🌟 Future Improvements

- Deploy on AWS / Render  
- Add Docker support  
- Improve UI design  
- Add model monitoring  

---

## 👨‍💻 Author
Pushp Kumar   
---
