# ⚽ **Soccer Match Analysis & Prediction** 🏆  

## 📌 **Overview**  
This script analyzes soccer match data from `soccer_matches.csv`, performs exploratory data analysis (EDA), and builds a **Random Forest model** to predict match results. The analysis includes visualizations of key match statistics and evaluates the model’s accuracy.  

---

## 📂 **Dataset Information**  
The dataset contains information about soccer matches, including:  
- **Home Team & Away Team** 🏟️ – Teams competing in each match.  
- **Goals Scored** ⚽ – Goals scored by home and away teams.  
- **Shots & Possession** 🎯 – Statistics on shots taken and ball possession.  
- **Passes Completed** 🔄 – Number of passes by each team.  

---

## 🔍 **Key Features & Analysis**  
1️⃣ **Data Preprocessing & Encoding**  
   - Encodes **team names** into numerical values.  
   - Creates a **match result column** (Home Win = 1, Draw = 0, Away Win = -1).  

2️⃣ **Exploratory Data Analysis (EDA)**  
   - **Boxplots** of key statistics (shots, possession) vs. match results.  

3️⃣ **Machine Learning Model (Random Forest Classifier)**  
   - Splits the dataset into **training (80%)** and **test (20%)** sets.  
   - **Standardizes** numerical features for better performance.  
   - Trains a **Random Forest model** to predict match results.  

4️⃣ **Model Evaluation**  
   - Computes **accuracy, classification report, and confusion matrix**.  
   - **Visualizes** the confusion matrix for better interpretation.  

---

## 📊 **Visualizations & Insights**  
📌 **Boxplots:** Show how key statistics (shots, possession) affect match results.  
📌 **Confusion Matrix:** Displays the model’s performance in predicting wins, draws, and losses.  

---

## 🛠️ **Requirements**  
Ensure you have the required Python libraries installed:  
```bash
pip install pandas scikit-learn seaborn matplotlib
```  

---

## 🚀 **How to Run the Script**  
1️⃣ Place the `soccer_matches.csv` file in the same directory as the script.  
2️⃣ Run the script using:  
```bash
python script.py
```  
3️⃣ View printed statistics, model performance metrics, and visualizations.  

---

## 🎯 **Future Enhancements**  
🔹 Add more features like **team rankings, player statistics, and match venue data**.  
🔹 Try different models like **Logistic Regression, XGBoost, or Neural Networks**.  
🔹 Optimize hyperparameters for better accuracy.  

---

📌 **Happy Analyzing & Predicting!** ⚽🚀