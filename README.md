# Group Activity: Predicting Diabetes with ML  
**Due:** December 1, 2025 — 9:00 AM  

---

## **Phase 1: Data Understanding & Exploration (EDA)**  
**Objective:** Understand the dataset's structure, identify potential issues, and visualize key relationships.

### **Tasks**

### **1. Load and Inspect**
- Load the dataset.  
- Check the number of rows and columns (observations and features).  
- Display the first five rows and check the data types of each column.  

### **2. Missing Data Check (The PIMA Trap)**
- The dataset represents missing values as **0** in several columns (e.g., *Blood Pressure, Glucose, BMI*).  
- For the columns **Glucose, Blood Pressure, Skin Thickness, Insulin, and BMI**, count how many zero values exist.  
- These zeros are typically placeholders for missing measurements.

### **3. Summary Statistics & Distribution**
- Generate a descriptive statistics summary for all features.  
- **Visualization Task:** Plot histograms of the key features (especially **Glucose** and **BMI**), colored by **Outcome (0 or 1)** to observe potential separation between diabetic and non-diabetic individuals.

---

## **Phase 2: Data Preprocessing & Feature Engineering**  
**Objective:** Clean the data and prepare it for machine learning.

### **Tasks**

### **1. Handling Missing Values**
- Decide on a strategy for the "missing" zero values identified in Phase 1.  
- **Recommended Strategy:** Replace zero values in key medical features with the **median** of that column (median is less sensitive to outliers).  
- Verify that the zero values have been successfully imputed.

### **2. Feature Scaling (Normalization/Standardization)**
- Explain why scaling is important for ML models.  
- Apply a **StandardScaler** (or similar) to all numerical input features.  
- *Do not scale* the target variable **Outcome**.

---

## **Phase 3: Model Training & Selection**  
**Objective:** Train and compare three different classification models.

### **Tasks**

### **1. Split the Data**
- Separate features (**X**) from the target (**y**).  
- Split into **Training (70%)** and **Testing (30%)** sets.

### **2. Model 1: Logistic Regression**
- Initialize and train a **Logistic Regression** model.

### **3. Model 2: K-Nearest Neighbors (KNN)**
- Initialize and train a **KNN classifier** (start with **K = 5**).

### **4. Model 3: Random Forest Classifier**
- Initialize and train a **Random Forest Classifier** (start with default parameters, e.g., 100 trees).

### **Discussion Point:**
Explain how **Random Forest** differs from **Logistic Regression**, and why it often achieves higher accuracy.  
*Hint: Ensemble learning reduces overfitting.*

---

## **Phase 4: Model Evaluation & Interpretation**  
**Objective:** Evaluate model performance and interpret the results.

### **Tasks**

### **1. Prediction**
- Use each trained model to generate predictions on the Test Set.

### **2. Evaluation Metrics**
- Calculate the **Accuracy Score** for all three models.  
- Generate and analyze the **Confusion Matrix** for the best-performing model.  
- **Focus:** Explain the meaning of **False Negatives (FN)** in a medical context.

### **3. Model Interpretation**
- Use the model's built-in **Feature Importance** or **Coefficients** attribute.  
- Identify the **top 3 most important features** according to the model.

---

## **Required Tools**
- **Python**  
- **Libraries:**  
  - `pandas` — data handling  
  - `numpy` — numerical operations  
  - `matplotlib` / `seaborn` — visualizations  
  - `scikit-learn` — ML models and scaling  

---
