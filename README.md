# Web Traffic Time Series Forecasting

A time-series forecasting project demonstrating an **iterative/nested forecasting workflow in R** using `modeltime`, `tidymodels`, and `timetk`.

The project uses historical daily Wikipedia web traffic data to build and compare multiple machine-learning forecasting models across several web pages. Each time series is modelled independently, evaluated on unseen test data, and assigned the model that performs best based on out-of-sample **Mean Absolute Error (MAE)**.

## Project Overview

The workflow covers the complete forecasting process:

- Data cleaning and transformation
- Exploratory time-series analysis
- Anomaly detection and treatment
- Calendar-based feature engineering
- Nested train/test splitting
- Training multiple forecasting algorithms
- Out-of-sample model evaluation
- Automated model selection for each time series
- Model refitting using complete historical data
- 90-day future forecasting with prediction intervals

The candidate models evaluated are:

- **XGBoost**
- **Random Forest**
- **K-Nearest Neighbors (KNN)**

The analysis is implemented using the `tidymodels`, `modeltime`, and `timetk` ecosystem.

## Project Structure

``` text
.
├── data
│   └── web_traffic_data.csv
├── web_traffic_time_series_forecasting.Rmd
├── web-traffic-time-series-forecasting.Rproj
└── www
    └── img
        └── cover.jpeg
```

The main analysis is contained in `web_traffic_time_series_forecasting.Rmd`, while the `data/` directory contains the dataset used for modelling.

## Data Source

The web traffic data used in this project was sourced from the **Web Traffic Time Series Forecasting competition dataset** available on Kaggle:

<https://www.kaggle.com/competitions/web-traffic-time-series-forecasting/data>

## Running the Project

Clone or download the repository, open:

``` text
web-traffic-time-series-forecasting.Rproj
```

Then open and render:

``` text
web_traffic_time_series_forecasting.Rmd
```

The required R packages are loaded within the analysis.

## Author

**George N. Mwangi**
