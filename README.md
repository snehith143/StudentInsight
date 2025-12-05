# 🎓 AI-Powered Student Performance Prediction System

A Machine Learning–powered web application that predicts student academic performance using behavioral, demographic, and academic indicators. Built with **Python**, **Streamlit**, and **Scikit-learn**, this project makes it easy for educators to identify at-risk students early and improve academic outcomes.

---

## ✨ Features

* 📤 Upload your own dataset (CSV)
* 🧹 Automatic data preprocessing
* 🤖 Train regression or classification ML models
* 📈 Visual performance metrics
* 🔮 Predict new student outcomes
* 💾 Save trained models as `.pkl`
* 📊 Built-in synthetic dataset
* 🧠 Optional SHAP explainability
* 🌐 Deployable on Replit, HuggingFace, or GitHub Codespaces

---

## 📂 Project Structure

```
├── main.py                          # Streamlit Application
├── requirements.txt                 # Dependencies
├── student_performance_dataset.csv  # Sample dataset
├── model.pkl                        # Trained model (auto-generated)
└── README.md                        # Project documentation
```

---

## 🧠 How It Works

### **1️⃣ Load Data**

* Upload CSV or use built-in demo data
* Preview dataset and summary statistics

### **2️⃣ Preprocessing**

* Missing value handling
* Categorical encoding
* Numeric scaling
* Train/test split

### **3️⃣ Model Training**

Supports two modes:

#### **Regression**

Predicts a student's final score (0–100)
Metrics:

* MAE
* RMSE
* R² Score

#### **Classification**

Predicts pass/fail (1 = pass)
Metrics:

* Accuracy
* F1-Score
* ROC-AUC

Algorithm used:

* Random Forest
* (Optional) XGBoost

### **4️⃣ Prediction**

* Enter new student details
* Get instant score or pass/fail prediction

### **5️⃣ Model Saving**

Exports trained model as `model.pkl`.

---

## 🛠️ Tech Stack

* Python
* Streamlit
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Joblib
* SHAP (optional)

---

## 📊 Dataset Details

A ready-to-use dataset is included:
**student_performance_dataset.csv**

It contains the following features:

| Column             | Description                           |
| ------------------ | ------------------------------------- |
| student_id         | Unique ID                             |
| attendance         | % of classes attended                 |
| study_hours        | Daily study hours                     |
| past_score         | Previous exam marks                   |
| parental_education | none / primary / secondary / tertiary |
| extracurricular    | yes / no                              |
| health             | good / average / poor                 |
| final_score        | Target for regression                 |
| pass               | Target for classification (0/1)       |

---

## 🚀 Installation & Running

### **1️⃣ Clone Repository**

```bash
git clone https://github.com/snehith143/StudentInsight/tree/main
```

### **2️⃣ Install Dependencies**

```bash
pip install -r requirements.txt
```

### **3️⃣ Run Streamlit App**

```bash
streamlit run main.py
```

The app runs at:

```
http://localhost:8501
```

---

## 🌐 Deployment Guide

### **▶ Replit**

1. Create new Replit (Python)
2. Upload project files
3. Set Run Command:

```
streamlit run main.py --server.port=8000 --server.address=0.0.0.0
```

### **▶ HuggingFace Spaces**

* Choose “Streamlit”
* Upload repository
* Deploy instantly

### **▶ GitHub Codespaces**

```
streamlit run main.py
```

---

## 📈 Example Model Performance

(Using demo dataset)

**Regression:**

* MAE: 3.4
* R² Score: 0.89

**Classification:**

* Accuracy: 92%
* F1 Score: 0.91
* ROC-AUC: 0.95

Actual numbers vary with your dataset.

---

## 🗺️ Roadmap

* [ ] Add LightGBM & SVM
* [ ] Add deep learning model (LSTM)
* [ ] Add student risk level prediction
* [ ] Add recommendation engine
* [ ] Add user authentication for teachers

---

## 🤝 Contributing

Contributions are welcome!

Steps:

1. Fork this repository
2. Create a new branch
3. Commit your changes
4. Open a pull request

---

## 📜 License

Released under the **MIT License**.

---

## 👤 Author

**Your Name**
GitHub: [https://github.com/your-username](https://github.com/snehith143)
