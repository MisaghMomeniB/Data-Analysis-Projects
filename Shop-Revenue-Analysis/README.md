# 📊 **Sales Data Analysis & Visualization** 🛍️  

## 📌 **Overview**  
This script performs an in-depth analysis of a sales dataset (`sales-data.csv`) using `pandas`, `seaborn`, and `matplotlib`. It extracts key insights about product pricing, stock levels, and supplier distributions, and visualizes important trends through various charts.  

---

## 📂 **Dataset Information**  
The dataset contains information about different products, including:  
- **Category** 🏷️ – The product category.  
- **Supplier** 🏭 – The supplier of the product.  
- **Price** 💲 – The price of the product.  
- **Stock** 📦 – The available stock quantity.  

---

## 🔍 **Key Features & Analysis**  
1️⃣ **Basic Statistics Summary**  
   - Total number of products.  
   - Number of unique categories and suppliers.  
   - Average product price and stock availability.  

2️⃣ **Identifying Extremes**  
   - Most and least expensive products.  
   - Products with the highest and lowest stock levels.  

3️⃣ **Correlation Analysis**  
   - Computes and visualizes the correlation between `Price` and `Stock`.  

4️⃣ **Visualizations**  
   📈 **Price Distribution Histogram** – Shows the spread of product prices.  
   📊 **Category Distribution Bar Chart** – Displays product counts by category.  
   🏭 **Supplier Distribution Bar Chart** – Highlights the number of products per supplier.  
   🔥 **Correlation Heatmap** – Depicts the relationship between numerical variables.  
   📦 **Price Distribution by Category (Boxplot)** – Analyzes price variations across categories.  
   🎯 **Price vs. Stock Scatterplot** – Reveals patterns between price and stock availability.  
   🥧 **Category Distribution Pie Chart** – Illustrates category proportions.  

---

## 📈 **Key Insights & Findings**  
🔹 Categories and suppliers with the highest number of products.  
🔹 Identification of high-value and low-stock products.  
🔹 Pricing trends and stock correlations.  
🔹 Outliers in product pricing across categories.  

---

## 🛠️ **Requirements**  
Ensure you have the following Python libraries installed:  
```bash
pip install pandas matplotlib seaborn
```  

---

## 🚀 **How to Run the Script**  
1️⃣ Place the `sales-data.csv` file in the same directory as the script.  
2️⃣ Run the script using:  
```bash
python script.py
```  
3️⃣ View printed statistics and generated charts.  

---

## 🎯 **Future Enhancements**  
🔹 Perform time-series analysis on sales trends.  
🔹 Predict stock depletion using machine learning models.  
🔹 Implement interactive dashboards for real-time analysis.  

---

📌 **Happy Analyzing!** 📊🚀