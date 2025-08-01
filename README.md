#  Electric Vehicle (EV) Data Analysis Project using Python

This project explores electric vehicle (EV) specifications and performance data using Python. The aim is to analyze key features like battery capacity, driving range, energy efficiency, and pricing to generate insights and recommendations for consumers.

---

##  Project Overview

The dataset includes technical and performance metrics of various electric vehicles (EVs) from leading brands such as Audi, Tesla, BMW, and Hyundai. The project performs:

- Data cleaning and filtering
- Exploratory data analysis
- Outlier detection
- Custom recommendation system
- Statistical comparison between car brands

---

##  Tools & Technologies

- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib**, **Seaborn**
- **SciPy** (for hypothesis testing)
- Jupyter Notebook / Colab

---

##  Dataset Highlights

Columns include:

- Car Make & Model
- Price (PLN), Battery Capacity, Range (WLTP)
- Engine Power, Torque, Drive Type, Braking System
- Acceleration, Charging Power, Energy Consumption
- Boot Capacity, Seating, Speed, etc.

---

##  Key Tasks Performed

### 1. EV Filtering & Grouping
- Selected EVs under **350,000 PLN** with a range ≥ **400 km**
- Grouped by manufacturer and computed average battery capacity

### 2. Outlier Detection
- Used IQR method to detect outliers in energy consumption  
→ **No extreme outliers found**

### 3. Visualization
- Created scatter plots (e.g., battery capacity vs. range)

### 4. Custom Recommendation System
- Implemented an `EVRecommender` class:
  ```python
  recommender = EVRecommender(df)
  recommender.recommend(budget=300000, min_range=350, min_battery=60)
