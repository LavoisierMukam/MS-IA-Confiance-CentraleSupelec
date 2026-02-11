# Data Analysis & Visualization - Lab 2
**Student:** Lavoisier MUKAM  
**Institution:** CentraleSupélec (MS AI for Trustworthy Systems)

---

## 📌 Project Overview
This project focuses on advanced data visualization and time series analysis using Python. It explores real-world datasets to identify patterns, clean inconsistent data, and demonstrate physical correlations through visualization.

## 🛠️ Key Skills Demonstrated
* **Scientific Visualization:** Multi-axis plotting with `Matplotlib` and interactive animations with `Plotly`.
* **Time Series Engineering:** Handling `DateTimeIndex`, frequency resampling, and window slicing in `Pandas`.
* **Data Integrity (Trustworthy AI):** Cleaning missing values (`NaN`) and handling sensor errors (e.g., specific codes like `-9999`).
* **Feature Extraction:** Transforming raw timestamps into actionable features (hour, day of week, etc.).

---

## 📊 Main Analyses

### 1. NYC Taxi Trip Patterns
* **Interactive Analysis:** Using Plotly to visualize how taxi activity fluctuates between weekdays (commuting peaks) and weekends.
* **Dynamic Modeling:** Animation of average fare amounts to detect anomalies or trends over time.

### 2. Household Power Consumption vs. Temperature
The core of this lab is the correlation between energy demand and climate.
* **Dataset:** Individual household electric power consumption (UCI).
* **Methodology:** * Merged electrical data with historical weather data.
    * Handled the 1/10th degree scaling and missing values in temperature logs.
    * Implemented a **Twin Axis (Dual-Y)** plot to overlay different units (kW vs. °C).

**Result:** A clear negative correlation was identified, confirming that electric heating is the primary driver of consumption for the analyzed household during the winter-to-spring transition.



---

## 🚀 How to Run
1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/votre-username/lab2-data-viz.git](https://github.com/votre-username/lab2-data-viz.git)
    ```
2.  **Install dependencies:**
    ```bash
    pip install pandas numpy matplotlib plotly
    ```
3.  **Ensure data files are in the same directory:**
    * `nyc_taxi.csv`
    * `household_power_consumption.txt`
    * `TG_STAID011249.txt`
4.  **Run the Jupyter Notebook:**
    ```bash
    jupyter notebook
    ```

---

## 📝 Conclusion
This lab demonstrates the importance of data cleaning and proper indexing in time series. Being able to visualize the physical relationship between temperature and power usage is a crucial step towards building explainable and trustworthy AI models for energy management.
