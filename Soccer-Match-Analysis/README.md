---

# Football-Match-Outcome-Prediction ⚽️

This project predicts the outcomes of football matches (home win, away win, or draw) using machine learning techniques. By leveraging historical match data, we train a Random Forest model to classify match results based on features like shots, possession, and passes. 

## Project Overview 📊

Football matches have unpredictable outcomes, but by analyzing historical data, we can make informed predictions. In this project, we use data from various football games to predict the result of future matches. The core steps of this project include data preprocessing, exploratory data analysis (EDA), model training, and evaluation.

### Features in the Dataset 🏟️:
- **home_team**: Name of the home team.
- **away_team**: Name of the away team.
- **home_goals**: Number of goals scored by the home team.
- **away_goals**: Number of goals scored by the away team.
- **shots_home**: Number of shots by the home team.
- **shots_away**: Number of shots by the away team.
- **possession_home**: Possession percentage of the home team.
- **possession_away**: Possession percentage of the away team.
- **passes_home**: Number of passes by the home team.
- **passes_away**: Number of passes by the away team.

## How It Works 🔍

1. **Data Preprocessing**:
   - We load the dataset and convert categorical data (team names) into numeric values.
   - We then calculate the result of the match (home win, away win, or draw) based on the goals scored by both teams.

2. **Exploratory Data Analysis (EDA)**:
   - We explore relationships between match statistics (like shots and possession) and match outcomes using **boxplots**.

3. **Model Building**:
   - We build a **Random Forest model** using the selected features to predict the match outcome.
   - The model is trained on historical data, and the accuracy of the predictions is evaluated on test data.

4. **Evaluation**:
   - We assess the model’s performance using **accuracy score**, **classification report**, and **confusion matrix**.

## Steps to Run the Project ⚙️

### 1. Clone the repository:
```bash
git clone https://github.com/your-username/Football-Match-Outcome-Prediction.git
```

### 2. Install Dependencies:
Make sure to have Python installed, and then install the necessary dependencies:
```bash
pip install -r requirements.txt
```

### 3. Run the Code:
Run the `football_prediction.py` script to start the analysis:
```bash
python football_prediction.py
```

## Code Explanation 📜

### 1. **Loading and Preprocessing Data**:
```python
df = pd.read_csv("soccer_matches.csv")
label_encoder = LabelEncoder()
df['home_team_encoded'] = label_encoder.fit_transform(df['home_team'])
df['away_team_encoded'] = label_encoder.fit_transform(df['away_team'])
df['result'] = df.apply(lambda row: 1 if row['home_goals'] > row['away_goals'] else (0 if row['home_goals'] == row['away_goals'] else -1), axis=1)
```
We load the CSV file containing historical match data and then encode the team names into numerical values. We also calculate the result of each match, where `1` represents a home win, `0` is a draw, and `-1` represents an away win.

### 2. **Exploratory Data Analysis (EDA)**:
```python
sns.boxplot(x='result', y='shots_home', data=df)
sns.boxplot(x='result', y='possession_home', data=df)
```
Here, we visualize how different match statistics (like shots and possession) are related to match outcomes using **boxplots**.

### 3. **Model Building and Prediction**:
```python
model = RandomForestClassifier(n_estimators=100, random_state=42)
model.fit(X_train_scaled, y_train)
y_pred = model.predict(X_test_scaled)
```
We build a **Random Forest classifier** to predict the match outcome based on the features. After training the model, we use it to make predictions on the test data.

### 4. **Model Evaluation**:
```python
accuracy = accuracy_score(y_test, y_pred)
print(f"Accuracy: {accuracy * 100:.2f}%")
```
We evaluate the performance of the model by calculating the **accuracy score** and displaying the **classification report** and **confusion matrix**.

## Results 📈

- **Accuracy**: The model's accuracy on the test data.
- **Classification Report**: Provides precision, recall, and F1-score for each class (home win, draw, away win).
- **Confusion Matrix**: Shows how many times the model predicted each class correctly or incorrectly.

## Conclusion 💡

By analyzing match statistics such as shots, possession, and passes, the model can predict football match outcomes with a reasonable degree of accuracy. This project demonstrates how machine learning can be applied to sports analytics to predict future events based on historical data.

---

**Feel free to contribute, provide feedback, or improve the model!** 🙌

---
