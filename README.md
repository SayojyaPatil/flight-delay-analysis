# Flight Delay Analysis for U.S. Domestic Flights

**Large-Scale Data Analytics | Apache Spark | PySpark | Machine Learning | Data Visualization**

An academic big-data analytics project examining U.S. domestic flight delays using Apache Spark, statistical analysis, and machine learning.

The project investigates airline punctuality, departure and arrival delays, airport-level patterns, and temporal variability, with an exploratory machine learning component for predicting departure delays.

## Project Overview

Flight delays affect airline operations, airport efficiency, and passenger experience. This project analyzes historical U.S. domestic flight records to identify patterns and explore factors associated with delays.

The analysis is organized into six stages:

1. **Data Cleaning:** Integrate flight, airline, and airport datasets using PySpark; handle missing values and engineer time-based features.
2. **Departure and Arrival Delays:** Analyze delay behavior at takeoff and landing.
3. **Airline Comparisons:** Compare airlines using delay duration, punctuality, and variability.
4. **Airport Analysis:** Examine delay patterns across origin airports and routes.
5. **Temporal Variability:** Investigate how delays change across departure times.
6. **Machine Learning:** Evaluate regression models for exploratory delay prediction.

## Technology Stack

- **Big Data Processing:** Apache Spark, PySpark
- **Programming:** Python
- **Data Analysis:** Pandas, NumPy, SciPy
- **Visualization:** Matplotlib, Seaborn
- **Machine Learning:** Spark MLlib
- **Development:** Jupyter Notebook, Google Colab

## Dataset

The project uses three historical aviation datasets:

- `flights.csv` — Flight schedules, departure and arrival information, and delays
- `airlines.csv` — Airline names and identifiers
- `airports.csv` — Airport names, codes, and geographical information

The original dataset files are not included in this repository. Reproduction requires obtaining the corresponding source data and updating notebook file paths.

## Key Findings

- Delays varied significantly by airline, airport, and departure time.
- Afternoon and evening flights exhibited greater delay exposure than early-morning flights.
- Airport delay totals were influenced by traffic volume, while delay variability offered additional insight into operational reliability.
- Airline comparisons revealed differences in average delay durations and punctuality.

These findings describe the historical data analyzed in the original academic project and should not be interpreted as current airline performance rankings.

## Machine Learning Evaluation

Three Spark MLlib regression models were evaluated:

| Model | Test RMSE (minutes) |
|---|---:|
| Linear Regression | 37.98 |
| Decision Tree Regressor | 40.86 |
| Gradient Boosted Trees | 41.81 |

Linear Regression produced the lowest recorded test RMSE among the evaluated models. However, predictive performance was limited, with a negative recorded test R².

**Important:** These figures are preserved from the original academic analysis. The models are exploratory and have not been validated for production flight-delay forecasting.

## Project Notebooks

The original eight notebooks are preserved without changes to their calculations, figures, or machine learning results.

| Stage | Notebook |
|---|---|
| Data Cleaning — Part A | [Part 1A](notebooks/PART%201-%20DATA%20CLEANING%28a%29.ipynb) |
| Data Cleaning — Part B | [Part 1B](notebooks/PART%201-%20DATA%20CLEANING%28b%29.ipynb) |
| Data Cleaning — Part C | [Part 1C](notebooks/PART%201-%20DATA%20CLEANING%28c%29.ipynb) |
| Departure and Arrival Delays | [Part 2](notebooks/PART%202%20-Delays%2CTakeoff%20and%20Landing.ipynb) |
| Airline Comparison | [Part 3](notebooks/PART%203%20-COMPARING%20AIRLINES.ipynb) |
| Airport Analysis | [Part 4](notebooks/PART%204-Relation%20Between%20Origin%20Airports.ipynb) |
| Temporal Variability | [Part 5](notebooks/PART%205%20-%20TEMPORAL%20VARIABILITY%20OF%20DELAYS.ipynb) |
| Machine Learning Predictions | [Part 6](notebooks/PART%206-FINAL%20PREDICTIONS%20USING%20ML.ipynb) |

The notebooks document the original academic workflow. Execution requires access to the original datasets and compatible software dependencies.

## Reproducibility

The repository documents the original analytical workflow. Full reproduction requires the original datasets, compatible Python and Spark dependencies, and adjustments to notebook-specific Google Colab or local file paths.

The saved notebooks are provided as records of the original project, rather than as a verified, one-command executable pipeline.

## Academic Context and Contributions

Developed as a collaborative project for **CIS-557: Introduction to Big Data**, University of Michigan–Dearborn.

**Project team:** Shrenik Jadhav, Vrunda Kadam, Sayojya Patil, Aniket Khedkar, and Sidharth Kalyan Ram.

**Sayojya Patil's documented contributions:**
- Data collection
- Temporal variability analysis of flight delays
- Data visualization

The full project reflects the combined contributions of the academic team.

## Limitations and Future Improvements

- Historical observations may not reflect current aviation conditions.
- Dataset availability and notebook-specific paths affect reproducibility.
- Predictive accuracy was limited in the original experiments.
- Additional features such as weather, congestion, and operational conditions could improve future modeling.
- A time-aware validation strategy would be valuable for subsequent experiments.

## Project Status

**Completed academic research and analytics project.**

Original notebooks and results preserved for documentation and portfolio purposes.
