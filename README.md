# 💻 Laptop Price Predictor - Machine Learning Project with Web App

This project is a machine learning based **Laptop Price Predictor** with a **web application** frontend built using **Flask**. The model predicts laptop prices based on user selected specifications such as RAM, CPU type, GPU type, brand, screen features and more.

---

## 📌 Project Overview

- 📊 Dataset Source: [Kaggle - Laptop Price Dataset](https://www.kaggle.com/)
- 🔧 ML Techniques Used:
  - Data cleaning and preprocessing
  - Feature engineering
  - Normalization and encoding
  - Model building & evaluation
  - Hyperparameter tuning
- 🌐 Web Application:
  - Developed using **Flask** for backend
  - Frontend includes `index.html` and `styles.css`
  - Users interact via a web form to input laptop features and get price predictions

---

## 🧠 Models Implemented

The following regression models were trained and compared:
- 🔹 **Linear Regression**
- 🔹 **LASSO Regression**
- 🔹 **Decision Tree Regressor**
- 🔹 **Random Forest Regressor** ✅ *(Best Accuracy)*

➡️ The **Random Forest Regressor** gave the best performance and was selected as the final model. It is 82%

---

## ⚙️ Steps Followed for Model Building

1. **Dataset Loading**  
   - Downloaded the CSV dataset from Kaggle  
   - Loaded it using `pandas.read_csv()`

2. **Library Installation & Setup**  
   - Created and activated a virtual environment  
   - Installed required libraries: `numpy`, `pandas`, `scikit-learn`, `flask`

3. **Data Preprocessing**
   - Handled mixed type and messy data (CPU, GPU, screen resolution, etc.)
   - Extracted features such as Touchscreen, IPS Display, Screen Size...
   - Encoded categorical variables 

4. **Feature Scaling & Normalization**
   - Applied normalization and encoding techniques

5. **Model Training & Selection**
   - Trained Linear Regression, LASSO, Decision Tree, and Random Forest models
   - Selected Random Forest based on highest accuracy
   - Performed hyperparameter tuning using GridSearchCV

6. **Model Exporting**
   - Saved the final model as a `.pkl` file using `joblib`

---

## 🌐 Web Application Details

- Backend built with **Flask** (`app.py`)
- Frontend includes:
  - `index.html` (web form for user input)
  - `styles.css` (styling for UI)
- Users select laptop specifications such as Brand, RAM, Weight, Screen Type, CPU, etc.
- On submitting, the app predicts and displays the laptop price

---

## 🚀 How to Run the Web Application

1. **Clone the repository:**
   ```bash
   git clone https://github.com/UdaraChamidu/laptop-price-predictor.git
   cd Laptop-Price-Predictor
2. **Open the web application folder and run:**
   ```bash
   python app.py
   
---

## 🖥️ Web Form Interface

<p align="center">
  <img src="https://github.com/user-attachments/assets/f48ea3e4-ede3-487f-b380-beff05b12229" width="45%" />
  <img src="https://github.com/user-attachments/assets/159227d9-e2b8-434f-9dfe-483db504ee3f" width="45%" />
</p>




