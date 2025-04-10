# ML-Project-Big-Mart-Sales-Prediction:
Here's a well-organized and properly written project description of the **Big Mart Sales Prediction using Machine Learning** project:

---

## 📊 Big Mart Sales Prediction using Machine Learning

### 🗂️ Dataset Overview:
This project aims to predict the sales of products in various outlets of Big Mart using machine learning. The dataset used is a CSV file containing **8,523 rows and 12 columns**, with both categorical and numerical features.

---

### 🧰 Libraries and Dependencies Used:
- **NumPy**: For numerical computations  
- **Pandas**: For data manipulation and analysis  
- **Matplotlib & Seaborn**: For data visualization  
- **Scikit-learn**:  
  - `train_test_split`: For splitting the dataset into training and testing sets  
  - `r2_score`: For evaluating the model's performance (since the target variable is continuous)  
- **XGBoost**:  
  - `XGBRegressor`: For building the prediction model  
- **LabelEncoder** (from sklearn): For converting categorical labels to numeric form

---

### 🧹 Data Preprocessing:
- **Handling Missing Values**:
  - `Item_Weight`: Missing values were filled with the **mean** of the column using the `fillna()` function.
  - `Outlet_Size`: Missing values were replaced with the **mode** of the column with respect to the `Outlet_Type` using `pivot_table` and `lambda` functions for more precise imputation.
  
- **Label Encoding**:  
  Categorical features were transformed into numeric format using **Label Encoding** with `LabelEncoder` from `sklearn.preprocessing`.

---

### 📊 Data Visualization:
- **Distribution Plots**:  
  Used to visualize the distribution of **numerical features**.
- **Count Plots**:  
  Used to analyze the frequency of **categorical features**.
- Libraries used: `matplotlib` and `seaborn`

---

### 🧠 Model Training:
- The dataset was split into **training** and **testing** sets using `train_test_split`.
- An **XGBRegressor model** from the XGBoost library was used for prediction.
  
---

### 📈 Model Evaluation:
- **Training Score**: 87.26%
- **Testing Accuracy (R² Score)**: 54.75%

---

### ✅ Conclusion:
The model performs reasonably well on training data but shows room for improvement on unseen (test) data, indicating potential **overfitting**. Further model tuning and feature engineering could improve the test performance.

---

### 📁 Project Highlights:
- Efficient data cleaning and preprocessing using pandas and NumPy.
- Comprehensive data visualization using Seaborn and Matplotlib.
- Applied label encoding for handling categorical variables.
- Used a powerful gradient boosting model (`XGBRegressor`) for regression.
- Evaluated using R² Score appropriate for regression tasks.

---
