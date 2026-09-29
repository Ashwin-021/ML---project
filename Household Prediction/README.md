# ⚡ Household Energy Consumption Analysis

## 📌 Project Overview

This project analyzes **household energy consumption data** to understand electricity usage patterns and identify factors that influence energy consumption.

The dataset contains information about different households, daily energy consumption, household size, average temperature, air-conditioner usage, and peak-hour electricity consumption.

Python and data analysis libraries are used to **clean, explore, analyze, and visualize** the dataset.

---

## 🎯 Objectives

* Analyze daily household energy consumption.
* Understand the relationship between household size and energy usage.
* Study the impact of temperature on electricity consumption.
* Compare energy consumption between households with and without AC.
* Analyze peak-hour energy usage.
* Identify important patterns and trends in household electricity consumption.

---

## 📊 Dataset Information

The dataset contains **90,000 records** and **7 columns**.

| Column                   | Description                                            |
| ------------------------ | ------------------------------------------------------ |
| `Household_ID`           | Unique identifier for each household                   |
| `Date`                   | Date of energy consumption                             |
| `Energy_Consumption_kWh` | Total energy consumed by the household in kWh          |
| `Household_Size`         | Number of people in the household                      |
| `Avg_Temperature_C`      | Average temperature in Celsius                         |
| `Has_AC`                 | Indicates whether the household has an air conditioner |
| `Peak_Hours_Usage_kWh`   | Energy consumed during peak hours in kWh               |

---

## 🛠️ Technologies Used

* **Python**
* **Pandas**
* **NumPy**
* **Matplotlib**
* **Seaborn**
* **Jupyter Notebook / Google Colab**

---

## 🔍 Data Analysis

The project includes the following analysis:

### 1. Data Understanding

* Dataset shape and structure
* Column information
* Data types
* Statistical summary
* Duplicate and missing-value checking

### 2. Data Cleaning

* Handling missing values
* Checking duplicate records
* Converting the `Date` column into datetime format
* Checking data consistency

### 3. Exploratory Data Analysis

The following relationships are explored:

* Energy consumption over time
* Energy consumption by household size
* Energy consumption vs. temperature
* Energy consumption of households with and without AC
* Peak-hour energy usage
* Household-level consumption patterns

### 4. Data Visualization

Visualizations include:

* 📈 Line charts for energy consumption trends
* 📊 Bar charts for household comparisons
* 📉 Scatter plots for temperature and energy consumption
* 🔥 Heatmaps for correlation analysis
* 📦 Box plots for distribution analysis

---

## 📁 Project Structure

```text
Household-Energy-Consumption-Analysis/
│
├── Dataset/
│   └── household_energy_consumption.csv
│
├── Notebook/
│   └── Household_Energy_Consumption_Analysis.ipynb
│
├── Output/
│   ├── energy_consumption_trend.png
│   ├── household_size_analysis.png
│   ├── temperature_vs_energy.png
│   ├── ac_consumption_analysis.png
│   └── correlation_heatmap.png
│
└── README.md
```

---

## 🚀 How to Run the Project

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/Household-Energy-Consumption-Analysis.git
```

### 2. Open the Project

```bash
cd Household-Energy-Consumption-Analysis
```

### 3. Install Required Libraries

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

### 4. Run the Notebook

```bash
jupyter notebook
```

Open:

```text
Household_Energy_Consumption_Analysis.ipynb
```

---

## 📈 Key Analysis Areas

The project focuses on understanding how different factors are associated with household energy consumption:

* **Household Size → Energy Consumption**
* **Temperature → Energy Consumption**
* **AC Availability → Energy Consumption**
* **Peak-Hour Usage → Total Energy Consumption**
* **Date → Energy Consumption Trends**

---

## 💡 Insights

The analysis can help identify:

* Household energy consumption patterns.
* Differences in electricity usage based on household size.
* The relationship between environmental temperature and electricity demand.
* Differences in consumption between AC and non-AC households.
* Peak-hour electricity usage patterns.

---

## 🔮 Future Improvements

This project can be extended by:

* Building an **energy consumption prediction model**.
* Using Machine Learning algorithms such as **Linear Regression, Random Forest, and XGBoost**.
* Creating an interactive **Power BI dashboard**.
* Performing time-series forecasting.
* Developing an energy-saving recommendation system.

---

