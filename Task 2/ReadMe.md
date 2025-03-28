**Intern:** Sumanth Gubbala  
**Intern ID:** CT12RAU  
**Company:** CodTech IT Solutions  
**Mentor:** Sravani  
**Duration:** 8 Weeks  


## **2️⃣ Predictive Analysis (House Price Prediction)**  
### **🔹 Problem Statement**  
Built a **machine learning model** to predict **house prices** based on features like **location, size, number of rooms, and amenities**.  

### **🔹 Dataset**  
- **Source:** Kaggle - House Price Prediction Dataset  
- **Size:** 14,619 records  

### **🔹 Approach**  
✔ **Data Preprocessing:** Handled missing values, feature scaling, and encoding categorical data  
✔ **Feature Engineering:** Selected **significant variables** like area, number of floors, and age of the house  
✔ **Model Training:** Used **Random Forest Regression** for price prediction  
✔ **Performance Metrics:**  
  - **Random Forest MAE**: 114839.29647742817  
  - **Random Forest R² Score**: 0.75  

### **🔹 Prediction System Function**
```python
def predict_price(input_features, model, scaler):
    input_scaled = scaler.transform([input_features])
    prediction = model.predict(input_scaled)
    return round(prediction[0], 2)
```

## **📌 Output Screenshots**  
![image](https://github.com/user-attachments/assets/b2cdb35a-4db8-4afd-bb58-61c6a8ed73f0)
