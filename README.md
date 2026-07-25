# Housing-Price-Analysis
## Background and Overview

This project explores a residential housing dataset to understand the key factors influencing property prices. The goal is to uncover meaningful patterns that can help in pricing strategy, investment decisions, and market understanding.

### The analysis focuses on:

- Property size (living area)
- Overall quality of construction
- Year built (age of property)
- Neighborhood characteristics
- Price per square foot trends

## Data Structure Overview

The dataset contains 1460 residential properties with multiple features describing house characteristics.

### Key Features:
- SalePrice – Target variable (£)
- GrLivArea – Above-ground living area (sqft)
- OverallQual – Overall material and finish quality
- YearBuilt – Year the house was constructed
- Neighborhood – Location of the property
- Price per Sqft – Engineered feature (SalePrice / GrLivArea)

### Data Processing Steps:
- Handled missing values
- Created new feature: Price per Sqft
- Detected and removed extreme outliers (top 1%)
- Segmented data for premium housing analysis (OverallQual > 5)

## Executive Summary

- Property size strongly influences price
Larger homes tend to have higher prices, with a strong positive correlation between living area and SalePrice.
- Quality is a major price driver
Higher OverallQual significantly increases property value, indicating strong buyer preference for well-built homes.
- Newer homes command higher prices
Recently built properties show a consistent increase in SalePrice, reflecting modern demand.
- Price per sqft is increasing over time
New homes are not only more expensive but also cost more per square foot, showing increasing market valuation.
- Premium segment shows stronger trends
For high-quality homes, the relationship between size and price is even stronger (~0.70 correlation).
- Outliers can distort insights
A small number of extremely high-priced properties affected trends, but removing the top 1% improved clarity.
- Certain neighborhoods show premium pricing patterns
Some areas have higher price per sqft despite fewer properties, indicating exclusivity and strong demand.

## Insights Deep Dive

- Size vs Price
Strong correlation between GrLivArea and SalePrice
Larger homes → higher value, especially in premium segment
- Quality Impact
Higher OverallQual leads to significantly higher prices
Quality plays a key role in premium housing markets
- YearBuilt Trends
Newer houses show a clear upward price trend
Reflects demand for modern construction and features
- Price per Sqft Analysis
Increasing trend over time
Premium homes command higher £/sqft
- Outlier Handling
Used 99th percentile filtering
Improved trend visibility and reduced noise

## Recommendations

- Focus on high-quality, larger homes
Developers should prioritise building well-constructed homes with larger living spaces to maximise value.
- Invest in modern housing projects
The increasing price per sqft suggests strong demand for newer properties.
- Target premium neighborhoods
Areas with high price per sqft and limited supply offer strong investment opportunities.

## Tools & Technologies

- Python (Pandas, NumPy)
- Data Visualization (Matplotlib, Seaborn)
- Jupyter Notebook
