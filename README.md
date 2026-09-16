# NYC Taxi Operations Analytics

## 📌 Project Overview

This project analyses NYC Yellow Taxi trip data to identify demand patterns, fare trends, high-traffic zones and operational opportunities for improving taxi routing, dispatching and vehicle utilization.

The analysis uses a sampled subset of the 2023 NYC Yellow Taxi dataset and combines data preparation, data cleaning, exploratory data analysis, geospatial analysis and operational recommendations.

## 🎯 Business Objective

The main objectives of this project are to:

- Understand taxi demand patterns across hours, days and months.
- Identify busy hours and high-demand pickup and drop-off zones.
- Analyse the relationship between trip distance, fare and tips.
- Compare weekday and weekend traffic patterns.
- Identify slow routes and traffic-related operational inefficiencies.
- Analyse fare and tip patterns across passenger counts and vendors.
- Examine nighttime demand and revenue contribution.
- Analyse surcharge patterns.
- Develop data-driven recommendations for routing, dispatching, vehicle positioning and pricing.

## 📊 Dataset

The analysis uses the **NYC Yellow Taxi 2023 dataset**.

Due to the size of the original dataset, a 0.7% sample was taken from the monthly files and combined for analysis.

The resulting sample dataframe contains:

- **266,084 rows**
- **22 columns**

The dataset contains information related to:

- Pickup and drop-off timestamps
- Trip distance
- Trip duration
- Passenger count
- Fare amount
- Tip amount
- Total amount
- Payment type
- Pickup and drop-off location IDs
- Vendor information
- Surcharges
- Airport fees

**Dataset:** [NYC Taxi Operations Analytics Dataset](https://www.kaggle.com/datasets/gayatribehera5474/dataset-for-nyc-taxi-operations-analytics)

## 🛠️ Tools & Technologies

- Python
- Pandas
- NumPy
- PySpark
- Matplotlib
- Seaborn
- GeoPandas
- Jupyter Notebook
- NYC Taxi Zone Shapefile

## 🔄 Project Workflow

```text
NYC Yellow Taxi Dataset
          ↓
Data Sampling & Monthly File Combination
          ↓
Data Cleaning & Preparation
          ↓
Missing Value Treatment
          ↓
Outlier Handling
          ↓
Exploratory Data Analysis
          ↓
Demand & Revenue Analysis
          ↓
Geospatial Zone Analysis
          ↓
Route & Traffic Analysis
          ↓
Operational Analysis
          ↓
Business Insights & Recommendations
```

## 🔍 Analysis Performed

### 1. Data Preparation

- Loaded the NYC Yellow Taxi monthly datasets.
- Applied 0.7% sampling to manage the large dataset.
- Combined monthly files into a single analytical dataframe.
- Created a sampled Parquet dataset containing 266,084 rows and 22 columns.
  
### 2. Data Cleaning
- Removed unnecessary index and date/hour columns.
- Combined duplicate airport fee columns.
- Analysed missing-value proportions.
- Handled missing values in passenger count, RatecodeID and congestion surcharge.
- Removed invalid payment codes.
- Filtered unrealistic trip distances and fares.
- Examined zero and negative values in key numerical fields.
  
### 3. Exploratory Data Analysis

Analysed:

- Hourly taxi pickup distribution.
- Daily pickup patterns.
- Monthly pickup patterns.
- Monthly revenue trends.
- Quarterly revenue contribution.
- Trip distance and fare relationships.
- Fare and trip-duration relationships.
- Passenger count and fare relationships.
- Tip amount and trip-distance relationships.
- Payment type distribution.

### 4. Geospatial Analysis
  Used taxi-zone shapefile data with GeoPandas to:

- Merge zone information with trip data.
- Calculate trips by pickup zone.
- Calculate trips by drop-off zone.
- Visualise trip density across NYC taxi zones.
- Identify high-traffic pickup and drop-off locations.

### 5. Operational Analysis
  Analysed:

- Average speed across routes.
- Busiest hours.
- Weekday vs weekend traffic.
- Top pickup and drop-off zones.
- Pickup-to-drop-off ratios by zone.
- Nighttime traffic patterns.
- Daytime vs nighttime revenue share.
- Average fare per mile by passenger count.
- Average fare per mile by hour and day.
- Vendor-level fare differences.
- Distance-tiered fare differences.
- Tip percentages.
- Passenger-count patterns.
- Surcharge application patterns.

## 📈 Key Findings

  The analysis identified several important patterns:

- Fare amount shows a strong positive relationship with trip distance.
- Taxi demand increases during weekday rush hours.
- Weekend activity shows relatively higher late-night demand.
- Airport and Midtown areas show high pickup and drop-off density.
- Most trips involve 1–2 passengers.
- Credit card payments dominate the payment-type distribution.
- The analysis identified differences in fare-per-mile patterns between vendors.
- Q3 represented the largest quarterly share of the analysed revenue.
- Nighttime trips contributed approximately 12.25% of revenue in the analysed data, while daytime trips contributed approximately 87.75%.

## 💡 Business Insights & Recommendations

Based on the analysis, recommendations were developed around:

### Demand-Aware Vehicle Allocation

Increase vehicle availability during identified peak demand periods and maintain coverage in important nighttime areas.

### Zone-Level Dispatching

Prioritise high-demand zones and airport corridors for vehicle allocation while considering targeted reallocation for under-served areas.

### Traffic-Aware Routing

Use route-speed analysis and congestion information to identify slower corridors and support more efficient routing.

### Driver Utilization

Prioritise nearby available vehicles for forecasted pickups to reduce unnecessary travel and idle time.

### Predictive Dispatching

Use historical hourly and monthly demand patterns to anticipate peak periods and plan vehicle distribution.

### Pricing Strategy

Use demand, distance, fare and congestion-related patterns to support data-driven pricing and surcharge decisions.

## 📊 Visualizations

The project includes visualisations covering:

- Hourly, daily and monthly taxi demand
- Revenue trends
- Fare vs distance
- Fare and trip duration
- Payment types
- NYC taxi-zone trip density
- Weekday vs weekend demand
- Pickup and drop-off zones
- Nighttime traffic
- Fare-per-mile analysis
- Vendor comparisons
- Tip percentages
- Surcharge patterns

## ▶️ How to Run
- Clone or download this repository.
- Install the required Python libraries.
- Open EDA_Assg_NYC_Taxi_Gayatri_Behera.ipynb using Jupyter Notebook or JupyterLab.
- Ensure the required NYC Taxi dataset files and taxi-zone shapefile are available in the expected location.
- Run the notebook cells sequentially.

## 📁 Project Structure
```text
NYC-Taxi-Operations-Analytics/
│
├── EDA_Assg_NYC_Taxi_Gayatri_Behera.ipynb
├── Report_NYC_Taxi_Operations_Gayatri_Behera.pdf
└── README.md
```

## 📌 Project Outcome

This project demonstrates an end-to-end data analytics workflow using large-scale NYC taxi trip data.

The analysis combines data preparation, cleaning, exploratory analysis, geospatial analysis and operational insights to identify patterns that can support:

- Taxi demand planning
- Vehicle positioning
- Routing
- Dispatching
- Pricing decisions

## 👩‍💻 Author
Gayatri Behera

Data Analytics | Python | SQL | Power BI | Machine Learning | Engineering Analytics
