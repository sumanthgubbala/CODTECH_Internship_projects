**Intern:** Sumanth Gubbala  
**Intern ID:** CT12RAU  
**Company:** CodTech IT Solutions  
**Mentor:** Sravani  
**Duration:** 8 Weeks

## **3️⃣ Dashboard Development (Power BI - COVID-19 Data Visualization)**  

# 🦠 COVID-19 Global Dashboard (Power BI)

## 📌 Project Overview
This project involves building an **interactive Power BI dashboard** to visualize the **COVID-19 pandemic's global impact**. The dashboard presents **total cases, deaths, recoveries, and active cases** across different countries using **various visualizations**.

## 📝 Description

### **🔹 Problem Statement**
The COVID-19 pandemic has significantly impacted the world, making it essential to **analyze trends and patterns** in the number of **cases, fatalities, and recoveries**. This project helps in understanding the spread of the virus globally.

### **🔹 Dataset**
- **Source:** Kaggle - COVID-19 Global Dataset
- **Contains:**  
  - Confirmed Cases  
  - Fatalities  
  - Recoveries  
  - Country-wise records  
  - Latitude & Longitude for mapping  

## 🚀 Project Workflow

### **Step 1: Data Cleaning & Transformation**
✔ Imported dataset into Power BI  
✔ Removed missing/null values  
✔ Standardized date formats  
✔ Created new calculated columns  

### **Step 2: Creating Key Performance Indicators (KPIs)**
Created **KPI Cards** for:
- ✅ **Total Cases**  
- ⚰ **Total Deaths**  
- 💖 **Total Recoveries**  
- 🔥 **Active Cases** (Calculated using DAX formula)

**DAX Formula for Active Cases:**
```DAX
ActiveCases = [ConfirmedCases] - [Fatalities] - [Recovered]
```

## **📌 Output Screenshots**

![image](https://github.com/user-attachments/assets/f34e56ce-f1a3-4b6a-b9ba-9570b5584053)

