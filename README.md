# Intellihack 44Below Weather Prediction Project

## Overview
This project aims to predict rainfall patterns using historical weather data. Various machine learning algorithms are leveraged to create a rainfall prediction model based on weather parameters such as temperature, humidity, wind speed, cloud cover, and atmospheric pressure.

## Data Description
The dataset (`weather_data.csv`) contains daily weather measurements from January 2023 to October 2023. The key features included are:
- **date**: Date of observation
- **avg_temperature**: Average temperature of the day
- **humidity**: Humidity level
- **avg_wind_speed**: Average wind speed
- **rain_or_not**: Target variable (Rain = 1, No Rain = 0)
- **cloud_cover**: Cloud cover percentage
- **pressure**: Atmospheric pressure

## Methodology
### Data Preprocessing
- Conversion of categorical target to binary values (Rain = 1, No Rain = 0)
- Missing value imputation using the mean strategy
- Outlier detection and capping for wind speed
- Feature engineering including lag features and interaction terms
- Data exploration through correlation analysis and distribution visualization

### Models Implemented
The project evaluates several machine learning models:
- Logistic Regression
- Decision Tree
- Random Forest
- Gradient Boosting
- XGBoost

Each model is evaluated using accuracy metrics and classification reports. The best-performing models were further optimized using `GridSearchCV`.

## Key Features
- Comprehensive exploratory data analysis (EDA) with visualizations
- Feature importance analysis to identify key predictors of rainfall
- Hyperparameter tuning for optimal model performance
- Forecasting rain probability for future dates (21-day forecast)

## File Structure
- `weather_data.csv` - Raw weather data used for model training
- `weather (2).ipynb` - Jupyter notebook containing all code for data processing, analysis, and modeling
- `44Below_Task1_Report1.pdf` & `44Below_Task1_Report2.pdf` - Detailed reports on methodology and findings

## Installation and Usage
### Requirements
- Python 3.x
- Libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`, `xgboost`

### Running the Project
1. Clone this repository:
   ```bash
   git clone <repository_url>
   ```
2. Install the required dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn xgboost
   ```
3. Open and run the Jupyter notebook:
   ```bash
   jupyter notebook "weather (2).ipynb"
   ```

## Results
The models achieved good accuracy in predicting rainfall events based on weather parameters. Feature importance analysis revealed that humidity and temperature are among the most significant predictors of rainfall.

## Future Work
- Incorporate additional external data sources
- Experiment with deep learning approaches
- Improve feature engineering techniques
- Extend forecasting capabilities beyond 21 days

