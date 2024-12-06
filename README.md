# 🌊 Predict Water Availability - ACEA Group

## Project Overview
Efficient water management is crucial for sustaining ecosystems and human activities. This project focuses on forecasting the hydrometric level of the Arno River, the primary water source for the Florence-Prato-Pistoia metropolitan area in Tuscany, Italy. Leveraging advanced time-series modeling and machine learning, the project aims to optimize water usage and ensure sustainable resource management.

---

## 📂 Project Structure

The project is organized as follows:

- `time_series_analysis.ipynb` - The main Python script.
- `app.py` - Python script.
- `explore.py` - A notebook to explore data, play around, visualize, clean, etc. 
- `utils.py` - This file contains utility code for operations like database connections.
- `requirements.txt` - This file contains the list of necessary python packages.
- `models/` - This directory should contain your SQLAlchemy model classes.
- `data/` - This directory contains the following subdirectories:
  - `interin/` - For intermediate data that has been transformed.
  - `processed/` - For the final data to be used for modeling.
  - `raw/` - For raw data without any processing.

*Note*: This project structure is a general guideline and may not be strictly followed in every case. The actual structure might vary depending on the project needs, team preferences, or specific workflows.

---

## Dataset
The dataset, provided by ACEA Group, includes daily measurements of:
- **Hydrometry**: River levels over time.
- **Rainfall**: Precipitation data.
- **Temperature**: Climatic factors influencing water availability.

The dataset contains missing and redundant data, which were carefully processed to enhance data quality and model reliability.

---

## Objective
The primary goal is to forecast the hydrometric levels of the Arno River using statistical and machine learning models to support water management decisions.

---

## 📈 Key Features

### Exploratory Data Analysis (EDA)
- Insightful visualizations of trends, seasonality, and autocorrelation.

### Data Preprocessing
- Addressed missing data using techniques like linear interpolation and pattern repetition.
- Removed redundant and irrelevant features to streamline the dataset.

### Feature Engineering
- Extracted temporal features (year, month, season, etc.) for better model interpretability.

### Modeling Approaches
1. **ARIMA & AutoARIMA**: Statistical time-series models for baseline performance.
2. **Prophet**: Leveraged external regressors like rainfall and temperature for enhanced predictions.

---

## 🛠️ Technologies Used

| **Category**         | **Libraries/Tools**            |
|-----------------------|---------------------------------|
| Programming Language  | Python                         |
| Data Manipulation     | Pandas, NumPy                  |
| Visualization         | Matplotlib, Seaborn            |
| Time Series Analysis  | Statsmodels, Pmdarima          |
| Machine Learning      | Prophet, Scikit-learn          |

---

## 📊 Performance Summary

| **Model**       | **MAE (Mean Absolute Error)** | **MSE (Mean Squared Error)** |
|------------------|------------------------------|------------------------------|
| ARIMA           | e.g., 0.418                  | e.g., 0.354                  |
| AutoARIMA       | e.g., 0.439                  | e.g., 0.371                 |
| Prophet         | e.g., 0.331                  | e.g., 0.287                  |

**Note**: Despite its ability to incorporate external regressors, Prophet consistently outperformed ARIMA-based models in capturing seasonal patterns and hydrometric variability.

---

## 🚀 Getting Started

### Requirements
- **Python 3.8+**
- Install the required libraries:
  ```bash
  pip install pandas numpy matplotlib seaborn statsmodels pmdarima prophet scikit-learn
How to Run
Clone the repository:

bash
Copy code
git clone https://github.com/username/predict-water-availability.git
cd predict-water-availability
Open the notebook:

Open src/time_series_analysis.ipynb in Jupyter Notebook or VSCode.
Follow the step-by-step analysis and model implementation.
Generate predictions: Use the Prophet model to forecast future hydrometric levels

## 🌟 Highlights
Sustainable Impact: This project demonstrates how predictive modeling can help manage natural resources more effectively.   
Reproducibility: Each preprocessing and modeling step is thoroughly documented.    
Open Source Contribution: Designed to serve as a template for time-series forecasting in environmental sciences.  
## 📬 Contact
Author: Nathan Harroch  
LinkedIn: [linkedin.com/in/username](https://www.linkedin.com/in/nathan-harroch-b11590196/)  
Email: nathan.harroch06@gmail.com  
Disclaimer: This project was developed for educational and research purposes and is not directly affiliated with ACEA Group.  