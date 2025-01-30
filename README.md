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
- Overall, Intel closing stock price increased over the year of 1998. There were fluctuations but not
 significant; end of year closing price hit the highest of $125.
![Stock Chart](https://github.com/pngo1997/Images/blob/main/VS1%20-%20Line%20graph%20stock%20price.png)  

---

### **2. GM Car Sales Packed Bubble Chart**  
📊 **Car Sales by Make & Model**  
- Bubble chart has a tailored color system for each car brand which allows viewer to put more focus on a specific division, aka. car Make. Each circle's color and size represents a sub-category.
![GM Treemap](https://github.com/pngo1997/Images/blob/main/VS1%20-%20Bubble%20chart%20car.png)  

---

### **3. Montana Reservation Population Growth**  
📈 **Stacked Bar Chart of Reservation Populations** 
-  Overall, the reservations population increased steadily during 1970-2000; specifically, a big jump between 1970 and 1980.
- Majority of time, all reservations have population growth over the years. Significantly, the Flathead Reservation and the Fort Peck Reservation and Off-Reservation Trust Land have higher population growth compared to others over the years. These two reservations were major contributors to the significant incremental change in 1980.

![Montana Population](https://github.com/pngo1997/Images/blob/main/VS1%20-%20Stacked%20bar%20chart%20population.png)  

---

### **4. Cell Phone Pricing Plan Analysis**  
📊 **Tree Map: Data Bandwidth vs. Price**  
- **Customer perspective**:  A tree map with phone plan count per company represents by the color area. Then within each area/company, we have subgroup tree map represents different Data GB and corresponding Price plan.
 • Darker color aims for higher prices, bigger area aims for more GB (proportionally coded). The graph also show phone plan options and information.
 • Withthis, by looking at the visualization, customer will pay more attention to bigger area, less clutter.  For example, looking at the graph we instantly notice highest GB phone plan of each company and perhaps make psychological decision on getting more expensive phone plans thus benefit the company.
![Cell Plans](https://github.com/pngo1997/Images/blob/main/VS1%20-%20Treemap%20phone%20service.png)

---

### Ppre-attentive Attributes
- Pre-attentive attributes are stand out visual patterns/objects that viewers can notice pretty much instantly (200ms after exposure to the visual) without needed to make an intentional observation effort.
- These attributes can be considered as a powerful visualization technique that if implemented correctly, it can strongly capture the audience's attention instantly; and efficiently convey the data message without much of an explanation.
- Several features that are commonly used for pre-attentive attributes are color, tilt, size, shape, proximity, and shadow direction. These attributes can be established by using combinations of these features, or just by a single feature itself. The goal is to ensure pre-attentive object standing-out from the rest of the visualization, also represents meaningful data. The implementation approach must be properly decided to get the best efficiency affect, yet not over-powering to viewer's eye.

### Weber’s Law
- Weber’s Law emphasizes that the human brain perceives differences in object magnitudes not solely based on their absolute values, but rather by quantifying the ratio of difference. To be specific, in observing two objects, the perceived difference is constantly proportional to the ratio between their magnitude, using the magnitude of the first/original object as a benchmark.
- Given this, it is important to include 0 in the numerical axis of a bar chart because our brain tends to look for a benchmark in determining the magnitude difference of items. Technical wise, the percentage increase with respect to the 0 benchmark in the bar chart, help to consciously decide which bar has 'greater magnitude' than the others.
