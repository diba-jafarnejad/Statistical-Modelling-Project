# Final-Project-Statistical-Modelling-with-Python

## Project/Goals
The goal of this project was to analyze the relationship between bike availability at bike stations and nearby points of interest (POIs) using data collected from the CityBikes and Yelp APIs. The aim was to build a regression model to predict bike availability based on POI characteristics and derive insights into what factors influence bike availability.

## Process
### Step 1: Data Collection
- Collected bike station data using the CityBikes API for the chosen city (Toronto).
- Queried the Yelp API to retrieve details about nearby POIs (e.g., restaurants, art galleries).

### Step 2: Data Preparation
- merged the data from both APIs.

### Step 3: Exploratory Data Analysis (EDA)
- Visualized the distribution of POI ratings, distances, and bike availability.
- Detected outliers.
- Analyzed correlations between features.

### Step 4: Regression Modelling
- Built a regression model using Python’s `statsmodels` module to predict the average number of bikes available at a station.
- Interpreted the regression outputs to identify significant and non-significant predictors.

### Step 5: Results Analysis
- Analyzed the model performance and derived insights about the relationship between bike availability and POI characteristics.

## Results
- **Comparative API Coverage**:
  - The Yelp API provided rich information on POIs, including ratings, categories, and locations.
  - The CityBikes API offered detailed data on bike station availability.

- **Model Insights**:
  - The **Number of POIs** near a station was a significant predictor of bike availability (p-value < 0.05).
  - **POI Rating** and **Distance to POIs** were not significant predictors.
  - The model's R-squared value was 0.146, indicating limited explanatory power.

## Challenges
- **Data Collection**:
  - Merging data from two APIs with differing structures was complex.

- **Modeling**:
  - The low R-squared value indicated that additional predictors were needed.
  - Residuals were not normally distributed, violating regression assumptions.

- **Technical Issues**:
  - API limit call.

## Future Goals
- **Enhance the Model**:
  - Experiment with advanced regression techniques or machine learning models.
  - Cleaning Data

- **Convert to Classification**:
  - Categorize bike availability into `Low`, `Medium`, and `High` classes and use classification models.

- **Expand Data Collection**:
  - Collect data over a longer period to account for temporal variations (e.g., time of day, seasonality).

---


