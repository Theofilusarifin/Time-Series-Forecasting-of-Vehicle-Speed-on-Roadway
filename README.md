# Time Series Forecasting of Average Vehicle Speed on a Roadway

## Introduction
This project explores data analysis and time series forecasting to understand average vehicle speed on a roadway, crucial for traffic management and congestion reduction.

## Data Preprocessing
- Extracted data from CSV files containing features like local time, road ID, start and end point IDs, and average speed.
- Handled null and duplicate values, ensuring data integrity.
- Fetched additional data via the Overpass API for road and point features.
- Transformed features like max speed, highway type, and point IDs for compatibility.
- Scaled features using Standard Scaler.

## Feature Engineering
- Separated date and time components for temporal analysis.
- Transformed dates into days of the week for analysis.
- Calculated distances using geographical coordinates.
- Removed redundant features.
- Conducted outlier removal based on road segments.

## Exploratory Data Analysis
- Analyzed correlations between features, revealing strong negative correlations between time and average speed.
- Examined speed violations compared to maximum speeds, identifying significant violations.
- Explored speed variations by day and hour, indicating higher speeds on weekends and lower speeds during weekdays.

## Modeling
- Utilized Random Forest algorithm with hyperparameter tuning.
- Achieved 89.52% accuracy within 2 minutes of training.

## Evaluation
- Mean Squared Error (MSE) = 6.22
- Mean Absolute Error (MAE) = 1.75
- Symmetric Mean Absolute Percentage Error (sMAPE) = 8.56%

## Conclusion
This project provides insights into traffic patterns and speed variations, contributing to informed decision-making in traffic management and urban planning.
