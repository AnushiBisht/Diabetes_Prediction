# 🩺 Diabetes Prediction using Machine Learning

A machine learning project that predicts whether a person is diabetic or not based on medical attributes using **Support Vector Machine (SVM)** classification.  
Built with Python, Scikit-learn, Pandas, and NumPy.

---

## 🚀 Features

- ✅ Diabetes prediction using medical data
- ✅ Data preprocessing and analysis
- ✅ Feature scaling using StandardScaler
- ✅ SVM classification model
- ✅ Accuracy evaluation
- ✅ Predict custom patient input

---

## 🛠️ Tech Stack

- **Python**
- **Pandas**
- **NumPy**
- **Scikit-learn**
- **Jupyter Notebook**

---

## 📂 Dataset

This project uses the **PIMA Indians Diabetes Dataset**.

### Features Used

- Pregnancies
- Glucose
- Blood Pressure
- Skin Thickness
- Insulin
- BMI
- Diabetes Pedigree Function
- Age

### Target Variable

| Value | Meaning |
|------|---------|
| 1 | Diabetic |
| 0 | Non-Diabetic |

---

## ⚙️ Installation

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/diabetes-prediction.git
cd diabetes-prediction
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

---

## ▶️ Run the Project

Start Jupyter Notebook:

```bash
jupyter notebook Diabetes_Prediction.ipynb
```

Run all notebook cells to:
1. Load the dataset
2. Preprocess and scale the data
3. Train the SVM model
4. Evaluate accuracy
5. Predict diabetes status

---

## 🧠 Machine Learning Workflow

### 📌 1. Data Collection & Analysis

The dataset is loaded using Pandas and analyzed for:
- Missing values
- Statistical summary
- Feature distribution

```python
import pandas as pd

diabetes_dataset = pd.read_csv('diabetes.csv')
```

---

### 📌 2. Data Preprocessing

Feature scaling is applied using:

```python
from sklearn.preprocessing import StandardScaler

scaler = StandardScaler()
```

---

### 📌 3. Train-Test Split

The dataset is divided into training and testing sets.

```python
from sklearn.model_selection import train_test_split
```

---

### 📌 4. Model Training

Support Vector Machine classifier is used.

```python
from sklearn import svm

classifier = svm.SVC(kernel='linear')
```

---

### 📌 5. Model Evaluation

Model performance is evaluated using:
- Training Accuracy
- Testing Accuracy

---

## 📊 Sample Prediction

```python
input_data = (5,166,72,19,175,25.8,0.587,51)

prediction = classifier.predict(input_data_reshaped)

if prediction[0] == 0:
    print("The person is not diabetic")
else:
    print("The person is diabetic")
```

---

## 📁 Project Structure

```bash
diabetes-prediction/
│
├── Diabetes_Prediction.ipynb
├── diabetes.csv
├── README.md
└── requirements.txt
```

---

## 📌 Future Improvements

- 🌐 Build a web app using Flask/FastAPI
- 🚀 Deploy the model online
- 📊 Add visualizations and dashboards
- 🧠 Experiment with advanced ML models
- 📱 Create a frontend UI for predictions

---

## 🤝 Contributing

Contributions are welcome!

1. Fork the repository
2. Create a new branch
3. Commit your changes
4. Push the branch
5. Open a Pull Request

---

## 👨‍💻 Author

**Anushi Bisht**

If you liked this project, give it a ⭐ on GitHub!
