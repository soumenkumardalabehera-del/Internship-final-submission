# Weather Pattern Visualization - Spatial-Temporal Analysis

## 📋 Project Overview :-

This project demonstrates **spatial-temporal data analysis** through a comprehensive visualization of weather patterns across multiple geographic regions over time. It combines meteorological data analysis, interactive mapping, time series forecasting, and statistical modeling to identify weather trends, correlations, and anomalies.

**Key Objectives:**
*   Analyze how weather changes across different regions and time periods.
*   Create interactive visualizations to show spatial-temporal weather patterns.
*   Implement a simple forecasting model for temperature prediction.
*   Identify extreme weather events and correlations between different weather variables.
*   Showcase skills in geospatial data science and temporal analysis for an academic or portfolio project.

## 🚀 Key Features

### Spatial Analysis
*   **Interactive Mapping**: Displays temperature, humidity, and precipitation data on interactive maps.
*   **Geographic Correlation**: Analyzes relationships in weather patterns between different cities.
*   **Regional Pattern Identification**: Visualizes distinct weather characteristics across various locations.

### Temporal Analysis
*   **Seasonal Trend Analysis**: Identifies and visualizes yearly weather cycles.
*   **Time Series Forecasting**: Predicts future temperatures using a linear regression model.
*   **Pattern Recognition**: Detects monthly, daily, and seasonal weather patterns.
*   **Extreme Event Detection**: Identifies and analyzes periods of extreme heat, cold, or precipitation.

### Advanced Visualizations
*   **Animated Weather Maps**: Shows the monthly progression of weather changes across the U.S.
*   **Interactive Dashboards**: Combines multiple plots for a comprehensive overview.
*   **Correlation Matrices**: Visualizes the statistical relationships between weather variables.

## 🛠️ Technical Stack

### Programming Language
*   **Python 3.8+**

### Core Libraries
*   **Data Processing & Analysis**: `pandas`, `numpy`
*   **Visualization & Mapping**: `matplotlib`, `seaborn`, `plotly`, `folium`
*   **Machine Learning & Statistics**: `scikit-learn`
*   **Geospatial Analysis**: `geopandas`, `contextily`

## 🧠 Models & Algorithms

### 1. Linear Regression Forecasting Model
A simple linear regression model is used for temperature forecasting.
*   **Purpose**: Predict future daily temperatures for a specific city.
*   **Features Used**: Day of the year, lagged temperature values (from the previous day and week), humidity, and pressure.
*   **Validation**: The model's performance is evaluated using Mean Squared Error (MSE) and the R² score on a test set.

### 2. Statistical Analysis
*   **Correlation Analysis**: A Pearson correlation matrix is used to measure the linear relationships between key weather variables like temperature, humidity, and precipitation.
*   **Extreme Event Detection**: Extreme weather events are identified using quantile-based thresholds (e.g., temperatures above the 95th percentile).

## 📊 Data Structure

The analysis is based on a structured dataset with the following columns:
*   `city`: Location identifier (e.g., 'New York')
*   `date`: Timestamp of the observation
*   `latitude`, `longitude`: Geographic coordinates
*   `temperature`, `humidity`, `precipitation`, `wind_speed`, `pressure`: Meteorological measurements

For the analysis, several features are engineered from the raw data, including `month`, `season`, and `day_of_year`.

## 🔧 Installation & Setup

1.  **Clone the repository:**
    ```
    git clone https://github.com/your-username/weather-pattern-analysis.git
    cd weather-pattern-analysis
    ```
2.  **Install the required packages:**
    ```
    pip install pandas numpy matplotlib seaborn plotly folium geopandas scikit-learn contextily requests
    ```
    For use in Google Colab, you can run `!pip install ...` for the packages above in a notebook cell.

## 📝 Usage

The project is structured as a Jupyter Notebook (`weather_analysis.ipynb`) or Python script.
1.  **Load Data**: Replace the sample data generation with your own dataset by loading a CSV file.
2.  **Run Analysis**: Execute the cells sequentially to perform data exploration, visualization, and modeling.
3.  **Customize**: Modify the city list, time ranges, and model parameters to tailor the analysis to your specific interests.
