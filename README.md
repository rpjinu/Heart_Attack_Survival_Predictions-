# Heart_Attack_Survival_Predictions-
ALL python jupyter notebook

<img src="https://github.com/rpjinu/Heart_Attack_Survival_Predictions-/blob/main/project_img.png">

# 🏥 Heart Attack Survival Prediction

## 📌 Project Overview
This project aims to predict heart attack survival outcomes using machine learning models. The dataset contains patient demographics, medical history, lifestyle factors, and healthcare access information to determine the probability of survival after a heart attack.

## 📂 Dataset Description
The dataset consists of **50,000 records** with the following features:

dataset link:-https://www.kaggle.com/datasets/rpjinu/heart-attack-survival-dataset/data

- **Demographics**: 🌎 Country, 🧑 Age, 👨‍⚕️ Gender
- **Medical Conditions**: 🫀 Cholesterol Level, 🔴 Blood Pressure, 💊 Diabetes, 🏋️ Obesity
- **Lifestyle Factors**: 🚬 Smoking History, 🍷 Alcohol Consumption, 🏃 Physical Activity
- **Lab Measurements**: 🩸 LDL Cholesterol, 🔬 Triglycerides
- **Risk & Health Factors**: ❤️ Heart Disease Risk, 💊 Medication Adherence
- **Environmental & Socioeconomic Factors**: 🌆 Urbanization Level, 🏥 Access to Healthcare, 🎓 Education Level, 💰 Income Level
- **Target Variable**: ✅ `Heart_Attack_Outcome` (Survived or Not Survived)

## 📊 Exploratory Data Analysis (EDA)
Key EDA steps performed:
- 📈 Distribution analysis of numerical and categorical features.
- 🔍 Correlation matrix to identify relationships between variables.
- 🏥 Feature importance analysis to determine key survival factors.

## 🛠️ Model Development
### 1️⃣ **Data Preprocessing**
- Handling missing values (e.g., imputation strategies).
- Encoding categorical features.
- Feature scaling (Standardization/Normalization).

### 2️⃣ **Feature Selection**
- Using correlation analysis and feature importance scores.
- Selecting the top **15 most relevant features** for model training.

### 3️⃣ **Model Training & Evaluation**
Several machine learning models were trained and evaluated:
- ✅ **Logistic Regression**
- ✅ **Random Forest**
- ✅ **XGBoost**
- ✅ **Neural Networks**

**Performance Metrics Used:**
- 🎯 Accuracy
- 📉 Precision & Recall
- 📊 F1-score & ROC-AUC Curve

## 🚀 Deployment
The final model is deployed as an **API using FastAPI & Streamlit**:
- 🌐 **FastAPI** serves as the backend.
- 🖥️ **Streamlit** provides a user-friendly interface.
- 🔄 Model inference is performed in real-time based on user inputs.

## 🏗️ Project Structure
```
📦 Heart_Attack_Survival_Prediction
├── 📁 data              # Raw & processed data
├── 📁 notebooks         # Jupyter Notebooks for EDA & Modeling
├── 📁 models            # Trained model files
├── 📁 src               # Source code for preprocessing & modeling
├── app.py              # Streamlit App for Deployment
├── requirements.txt    # Dependencies
└── README.md           # Project Documentation
```

## 📦 Installation & Setup
### 🔧 Requirements
Ensure you have Python installed. Then, install dependencies:
```bash
pip install -r requirements.txt
```

### 🚀 Run the Application
1. Start FastAPI Backend:
```bash
uvicorn src.api:app --reload
```
2. Launch Streamlit Frontend:
```bash
streamlit run app.py
```

## 🎯 Future Improvements
- 📈 Optimize model hyperparameters.
- 🤖 Implement deep learning models.
- ☁️ Deploy the model on cloud platforms like AWS/GCP.

## 📜 License
This project is open-source and available under the **MIT License**.

---
📩 For queries or contributions, feel free to reach out! 🚀
