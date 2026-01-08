Venezuela Oil Reserves Analysis
Project Overview
This project performs an exploratory data analysis (EDA) on a dataset detailing Venezuela's oil reserves. The goal is to understand the distribution of various oilfield characteristics, identify key trends, and analyze relationships between different numerical features.

Data Source
The dataset used for this analysis is venezuela oil reserves.csv.

Data Cleaning and Preparation
Before analysis, the following data cleaning and preparation steps were performed:

The Estimated_Recoverable_Reserves_Billion_Barrels column, which contained a range ('100.00-270.00'), was handled by converting it to a numeric type, with missing values (including the range converted to NaN) being imputed with '185' and then coerced to numeric.
The Year_Discovered column, which contained values like '1970s', was cleaned by removing the 's' and then converting to datetime objects, with invalid parsing resulting in NaT (Not a Time) values, which were not present in the final data.
Missing values were checked across the dataset, and no missing values were found after the initial cleaning steps.
Exploratory Data Analysis (EDA)
Several visualizations were created to explore the data:

1. Distribution of Production Capacity
A histogram showing the distribution of Production_Capacity_Barrels_Day revealed the frequency of different production capacities among the oilfields.
2. Count of Oil Grade Types
A count plot illustrated the distribution of Oil_Type_Grade, indicating the most common types of oil found in the reserves.
3. Proven Reserves by Basin Region
A bar plot displayed the Proven_Reserves_Billion_Barrels across different Basin_Regions, highlighting regions with the highest proven reserves.
4. Production Capacity by Year Discovered
A bar plot showed the Production_Capacity_Barrels_Day grouped by Year_Discovered, indicating how production capacity has evolved over the discovery years.
5. Box Plot of Production Capacity
A box plot for Production_Capacity_Barrels_Day was used to identify potential outliers and understand the spread of production capacity values.
Correlation Analysis
A correlation heatmap was generated for numeric columns (Proven_Reserves_Billion_Barrels, Estimated_Recoverable_Reserves_Billion_Barrels, and Production_Capacity_Barrels_Day) to visualize the relationships between these quantitative variables.
Key Findings (Example - based on typical analysis, specific findings would come from detailed observation of plots)
The 'Orinoco Belt' region appears to have the highest proven reserves.
'Extra Heavy Crude' is the most prevalent oil type.
There is a strong positive correlation between Proven_Reserves_Billion_Barrels and Estimated_Recoverable_Reserves_Billion_Barrels.
Production capacity seems to vary significantly across different discovery years, with some early discoveries showing high capacities, and a notable presence of high capacity fields discovered around 2007-2010.
