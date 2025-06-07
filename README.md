# 💻 Laptop Price Predictor - Machine Learning Project

This project is a machine learning-based **Laptop Price Predictor** built using Python. The model estimates the price of a laptop based on various user-selected specifications such as RAM, CPU type, brand, screen features, and more.

## 📌 Project Overview

- 📊 Dataset Source: [Kaggle - Laptop Price Dataset](https://www.kaggle.com/)
- 🔧 ML Techniques Used:
  - Data cleaning and preprocessing
  - Feature engineering
  - Normalization and encoding
  - Model building & evaluation
  - Hyperparameter tuning

## 🧠 Models Implemented

The following regression models were trained and compared:
- 🔹 **Linear Regression**
- 🔹 **LASSO Regression**
- 🔹 **Decision Tree Regressor**
- 🔹 **Random Forest Regressor** ✅ *(Best Accuracy)*

➡️ The **Random Forest Regressor** gave the best performance and was selected as the final model.

## ⚙️ Steps Followed

1. **Dataset Loading**  
   - Downloaded the CSV dataset from Kaggle  
   - Loaded it using `pandas.read_csv()`

2. **Library Installation**  
   - Required libraries: `numpy`, `pandas`, `scikit-learn`

3. **Data Preprocessing**
   - Handled mixed-type and messy data (e.g., CPU, GPU, screen resolution)
   - Extracted useful features like:
     - Touchscreen (binary)
     - IPS Display (binary)
     - Screen Size in inches
     - Pixel density (PPI)
     - Weight in kg
   - Encoded categorical variables (like Brand, CPU, etc.)

4. **Feature Scaling & Normalization**
   - Applied normalization and encoding techniques to prepare data for training

5. **Model Training**
   - Trained multiple models
   - Evaluated each using R² score

6. **Model Selection & Tuning**
   - Chose **Random Forest Regressor** based on highest accuracy
   - Applied **GridSearchCV** for hyperparameter tuning

7. **Model Exporting**
   - Final model saved as `.pkl` file using `joblib`
   - Ready for deployment or integration with UI

## 🧾 User Inputs (for prediction)

The model takes the following laptop features as input:
- ✅ RAM Size
- ✅ CPU Brand/Model
- ✅ Storage (HDD/SSD)
- ✅ Touchscreen (Yes/No)
- ✅ IPS Display (Yes/No)
- ✅ Screen Resolution
- ✅ Laptop Brand
- ✅ Laptop Weight

Based on these features, the model predicts the **price of the laptop** in euros or can be converted to other currencies (e.g., LKR).

## 🖥️ Sample Prediction Output

```python
Price in LKR : 716154.12
