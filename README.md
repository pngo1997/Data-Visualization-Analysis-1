# 🏗️ Data Visualization & Analysis Project  

## 📜 Overview  
This project covers **data visualization and analysis** using **Tableau and R**, focusing on stock market trends, GM car sales, Montana reservation populations, pre-attentive attributes, and cell phone pricing plans. The goal is to apply **data visualization best practices** to uncover patterns and insights.  

## 🎯 Problem Explanation  

### **1. Intel Stock Price Visualization**
📌 Dataset: **Intel-1998 Stock Data**  
- **Line Chart:** Closing price vs. date.  
- **Bar Chart:** Trading volume vs. date.  
- **Scatter Plot:** Trading volume vs. daily price range (`High - Low`).  

📊 **Tools Used:** R or Tableau  

### **2. GM Car Sales Analysis**
📌 Dataset: **gmcar_price.txt**  
- **Treemap:** Car price grouped by **Make & Model**.  
- **Packed Bubble Chart:** Sales volume for car models.  
- **Heatmap:** Number of cars sold per **Make & Type**.  
- **Comparison:** Differences between treemap & packed bubble chart.  

📊 **Tool Used:** Tableau  

### **3. Montana Reservation Population Growth**
📌 Dataset: **reservation70-00.xlsx**  
- **Data Preprocessing in Tableau:**  
  - Rename `1970*` field (remove `*`).  
  - Pivot year fields into **Year & Population** columns.  
  - Convert `Year` to **whole number** and create **Date field** using `makedate(Year,1,1)`.  
  - Filter out **Montana population**, keeping only reservations.  
- **Graphs:**  
  - **Line Chart:** Individual reservation population trends.  
  - **Stacked Area Chart:** Total reservation population over time.  

📊 **Tool Used:** Tableau  

### **4. Cell Phone Pricing Plans Visualization**
📌 Dataset: **Cell Phone Plans (Provided R Code)**  
- **Recreate & Improve a Cell Phone Pricing Graph in R.**  
- **Two different visualization approaches:**  
  1. **Compare Pricing Across Companies.**  
  2. **Analyze Relationship Between Data Bandwidth & Price.**  
- **Ensure clear communication of insights.**  

📊 **Tool Used:** R  

## 🚀 Technologies Used  
- **R (ggplot2)** – Stock analysis & cell phone plan visualization.  
- **Tableau** – GM car sales, reservation growth, and stock market visualization.  
- **Excel (Preprocessing)** – Data cleaning for Tableau.  

## 📊 Example Output  

### **1. Intel Stock Price Line Chart**  
📈 **Stock Closing Price vs. Date**  
![Stock Chart](https://github.com/pngo1997/Images/blob/main/VS1%20-%20Line%20graph%20stock%20price.png)  

---

### **2. GM Car Sales Packed Bubble Chart**  
📊 **Car Sales by Make & Model**  
![GM Treemap](https://github.com/pngo1997/Images/blob/main/VS1%20-%20Bubble%20chart%20car.png)  

---

### **3. Montana Reservation Population Growth**  
📈 **Stacked Bar Chart of Reservation Populations**  
![Montana Population](https://github.com/pngo1997/Images/blob/main/VS1%20-%20Stacked%20bar%20chart%20population.png)  

---

### **4. Cell Phone Pricing Plan Analysis**  
📊 **Tree Map: Data Bandwidth vs. Price**  
![Cell Plans](https://github.com/pngo1997/Images/blob/main/VS1%20-%20Treemap%20phone%20service.png)  
