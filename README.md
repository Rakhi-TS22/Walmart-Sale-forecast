# Walmart Capstone Project

## Summary
Walmart, a multinational retail corporation, faces challenges in managing its inventory effectively, leading to issues aligning product supply with varying consumer demand.

## Problem Statement
Walmart struggles with inventory management, causing difficulties in matching product supply with consumer demand fluctuations.

## Project Objective
The primary objective is to develop accurate sales prediction models using fbprophet to forecast sales for the retail store over a 12-week period. This will optimize inventory levels, ensuring alignment between anticipated demand and actual supply across all outlets.

## Data Overview
The dataset includes historical sales data, inventory levels, and relevant variables such as promotional activities, seasonal trends, and economic indicators across multiple outlets.

| Feature Name | Description       |
|--------------|-------------------|
| Store        | Store number      |
| Date         | Weekly date       |
| Weekly Sales | Sales by store    |
| Holiday_Flag | Holiday indicator |
| Temperature  | Sale day temperature |
| Fuel_Price   | Fuel cost         |
| CPI          | Consumer Price Index |
| Unemployment | Unemployment Rate |

## Data Pre-processing Steps
Pre-processing involves handling missing values, normalizing data, and encoding categorical variables.

## Exploratory Data Analysis (EDA)
- Check data summary and quality
- Examine basic statistics, missing values, and data types
- Ensure data integrity and cleanliness

## Algorithm Used: fbprophet
The prophet algorithm is chosen for its effectiveness in time-series forecasting, especially in scenarios with seasonal patterns and holidays influencing sales data.

## Motivation for Choosing the Algorithm
fbprophet handles various time-series forecasting challenges like seasonality, holidays, and trend changes. It offers simplicity and ease of use, suitable for quick implementation and interpretation.

## Assumptions
- Persistence of historical sales patterns
- Relevance of external factors (e.g., promotions, economic conditions)
- Stability of consumer behavior

## Model Evaluation and Techniques
Evaluation involves assessing accuracy metrics specific to fbprophet such as Mean Absolute Percentage Error (MAPE) and visual inspection of forecast plots. Cross-validation techniques and train-test splits validate model performance on unseen data.

**Score:** 5.43%
```python
import matplotlib.pyplot as plt
import seaborn as sns

plt.figure(figsize=(12, 3))
sns.lineplot(x='Date', y='Weekly_Sales', data=data)
plt.title('Weekly Sales Trends')
plt.show()
```
## Inferences
Evaluation results provide insights into forecasting model accuracy and reliability, guiding adjustments to the algorithm or data preprocessing steps for refinement.

## Weekly Sales Performance Analysis
### Sales Enhancement Recommendations
- **Special Offers Strategy:** Targeted offers for high-performing stores; tailor promotions for underperforming stores.
- **Inventory Management:** Adjust levels based on store sales patterns; focus on high-demand products in low-sales stores.
- **Staff Allocation:** Optimize based on sales trends; ensure adequate staffing during peaks.
- **Product Analysis:** Identify top-selling products in underperforming stores; increase stock for popular items.

## Predictive Analysis
Forecast sales across all stores for the next 12 weeks, considering store-wise and overall trends. Develop a holistic holiday sales strategy to maximize year-end trends.

## January Sales Boost Strategy
Initiate promotions and incentives to drive revenue at the year's start. Clear holiday inventory, offer loyalty incentives, and promote winter essentials.

## Future Possibilities
Explore advanced features of fbprophet, include additional external variables, and adapt the model for real-time forecasting. Continuous improvement and adaptation will enhance inventory management accuracy and responsiveness in the long term.

credit : Intellipaat dataset
code : Rakhi Tulaskar
