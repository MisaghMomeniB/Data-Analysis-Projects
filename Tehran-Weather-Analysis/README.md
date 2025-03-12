# Weather Data Analysis 🌦️📊

## Overview:
This Python script analyzes weather data and provides valuable insights through visualizations. It uses **pandas**, **matplotlib**, and **seaborn** to process and plot the data, showing trends in temperature, humidity, pressure, wind speed, and more. The script also includes a correlation matrix and frequency analysis of weather conditions.

---

## Features:

- **Data Overview** 🧐: Displays basic information and statistical summary of the dataset.
- **Trend Visualizations** 📈: 
  - Temperature, Humidity, Pressure, and Wind Speed trends over time.
- **Weather Condition Frequency** 🌤️: Shows a count of different weather conditions in the dataset.
- **Correlation Matrix** 🔢: Displays the correlation between various numeric weather factors.
- **Interactive Plots**: Clear, readable plots for effective data analysis.

---

## How It Works:

### 1. **Reading and Preprocessing the Data** 📂:
   - The script reads a CSV file containing weather data (temperature, humidity, pressure, wind speed, and weather conditions).
   - Converts the 'Date' column to datetime format for better handling of time-based analysis.

### 2. **Data Visualization** 🎨:
   - **Temperature Trends**: Line plot showing how temperature changes over time.
   - **Humidity Trends**: Visualizes the variation in humidity levels.
   - **Pressure Trends**: Shows atmospheric pressure fluctuations.
   - **Wind Speed Trends**: Illustrates the changes in wind speed.

   These trends are plotted in a 2x2 grid layout for better comparison.

### 3. **Weather Condition Frequency** 🌤️:
   - A **countplot** visualizes the number of days for each weather condition (e.g., sunny, rainy, cloudy).
   
### 4. **Correlation Matrix** 🔍:
   - The correlation between numeric columns like temperature, humidity, pressure, and wind speed is calculated and displayed in a **heatmap**.
   - This helps to identify relationships and dependencies between the factors.

---

## Requirements:
- Python 3.x
- Libraries:
  - pandas
  - matplotlib
  - seaborn

You can install the required libraries with the following command:
```bash
pip install pandas matplotlib seaborn
```

---

## Data Format:
The data should be in a CSV file with the following columns:
- **Date**: Date of the weather observation.
- **Temperature (°C)**: Temperature in Celsius.
- **Humidity (%)**: Percentage of humidity.
- **Pressure (hPa)**: Atmospheric pressure in hPa.
- **Wind Speed (km/h)**: Wind speed in kilometers per hour.
- **Weather Condition**: Description of the weather (e.g., Sunny, Rainy, Cloudy).

---

## Visualizations:

### 1. **Temperature Trends** 📊  
Displays how the temperature has changed over time.

### 2. **Humidity Trends** 💧  
Shows the fluctuation of humidity throughout the period.

### 3. **Pressure Trends** 🌪️  
Tracks the changes in atmospheric pressure.

### 4. **Wind Speed Trends** 🌬️  
Illustrates how wind speed varies.

### 5. **Weather Condition Frequency** 🌞🌧️🌤️  
Counts the occurrence of different weather conditions.

### 6. **Correlation Matrix** 🔢  
Visualizes relationships between numeric factors in the dataset.

---

## Example Output:

Here’s an example of the plots you will get from the script:

- **Temperature, Humidity, Pressure, and Wind Speed Trends** over time.
- **Weather Condition Frequency** bar chart.
- **Correlation Matrix** heatmap showing dependencies between various weather features.

---

## Contributions:
Feel free to fork this repo and submit issues or pull requests for improvements. Contributions are welcome! 🤝

---

Good luck with your weather data analysis! 🌈