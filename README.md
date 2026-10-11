# Car-Price-In-depth-Analysis-Using-Python
This project explores a car-price dataset to examine how vehicle characteristics relate to listed car prices. Using Python, I inspected the dataset, checked its quality, explored categorical values, and created visualisations to identify patterns between price and selected vehicle features.
The work is organised into two main stages: data inspection and cleaning checks, followed by exploratory data visualisation.

## Objectives
- Inspect the dataset's structure, data types, and descriptive statistics.
- Check for missing values and duplicate records.
- Explore unique values in selected categorical columns.
- Visualise the distribution of car prices.
- Examine how car price varies with engine size, horsepower, body style, drive-wheel type, engine location, fuel type, and door number.
- Communicate the patterns observed and identify areas for further analysis.
  
## Tools and Libraries
 - Python - analysis workflow
 - Pandas - data loading, inspection, and tabular analysis
 - NumPy - numerical computing
 - Matplotlib - plotting
 - Seaborn - statistical visualisation

## Methodology

1. Data inspection   
Pandas was used to load and inspect the dataset. The workflow included:
- Reviewing the dataset's data types and non-null counts with info().
- Checking the number of rows and columns with shape.
- Previewing records with head().
- Checking for duplicate rows with duplicated().
- Checking missing-value counts with isnull().sum().
- Reviewing numerical summaries with describe().
- Inspecting unique values in selected categorical columns.
  
These checks help assess data structure and quality before interpreting the visualisations.

The notebook contains checks for missing values and duplicates.

2. Exploratory visualisation
- Matplotlib and Seaborn were used to create charts for selected variables:
- Visualisation	Variables	Purpose
- Bar chart	was used to explore price values across body-style records
- Scatter plot was used to examine the association between engine size and price
- Histogram was used to inspect the distribution of listed car prices
- Count plot was used to compare the number of records in each fuel category
- Bar chart	was used to explore price values across drive-wheel records
- Scatter plot with regression line	was used to examine the relationship between horsepower and price
- Line plot	was used to compare price patterns across engine-location categories
- Count plot was used to compare the number of records by door-number category

## Findings Recorded in the Notebook
The following are the patterns described in the original notebook. They should be treated as preliminary observations rather than proof of causation.
1. Car body style: The notebook reports that hardtop vehicles appear more expensive and wagons less expensive. To support this conclusion robustly, compare mean or median price by body style rather than interpreting a bar chart of individual records.
2. Engine size and price: The scatter plot is interpreted as showing that higher engine sizes tend to be associated with higher prices.
3. Price distribution: The notebook reports that many listed prices fall between approximately 5,000 and 10,000. Confirm the interval and currency or price unit from the histogram and dataset documentation.
4. Fuel type: The count plot shows the relative number of records for each fuel type. The notebook reports more gas-powered than diesel-powered vehicles in the dataset; this does not by itself establish buyer preference.
5. Drive-wheel type: The notebook reports that rear-wheel-drive (RWD) vehicles are more expensive and four-wheel-drive vehicles are more affordable. Validate this by aggregating prices by drive-wheel category.
6. Horsepower and price: The scatter plot and regression line are interpreted as showing a positive association between horsepower and price.
7. Engine location: The notebook reports higher prices for rear-engine vehicles than front-engine vehicles. Check group sizes and summary statistics before drawing a firm conclusion.
8. Door number: The notebook's count plot shows record counts by door-number category, not prices. It therefore cannot establish whether door number affects price.

## Conclusion
This project demonstrates a Python workflow for inspecting a tabular dataset and using exploratory visualisations to investigate how vehicle characteristics relate to car prices. The notebook explores numerical features such as engine size and horsepower, alongside categorical features such as body style, fuel type, drive-wheel type, engine location, and door number.

The analysis provides a starting point for further investigation. A stronger next iteration would calculate group-level price summaries, quantify relationships, check outliers, and validate the findings before using them to support pricing decisions.
