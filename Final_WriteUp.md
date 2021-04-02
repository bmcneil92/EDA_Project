## A Fair Fare

Brandon McNeil

## Abstract
The goal of this project was to analyze MTA turnstile data and supplementary datasets in order to get a better understanding of the current ridership of NYC subways. I worked with MTA turnstile data in conjunction with open source geospatial data to provide median income information on subway station’s neighborhoods. After the data was effectively cleaned, I was able to produce visualizations using matplotlib.

##D esign
For this project, I “partnered” with a non-profit organization looking to analyze which New Yorkers would be most affected by “new” fare hikes the MTA has proposed. Using the geospatial datasets, I was able to gain additional insight into commuter backgrounds that could help propose effective talking points when fighting against the proposed fare hikes.

## Data
For the MTA turnstile dataset, I focused on two 3 month time periods - Dec2018-Mar2019, and Dec2020-Mar2021. Each time period includes over 2 million rows of data. A quirk of the data includes stations having a one to many relationship with column headers {CA}, {UNIT}, and {SCP}. 
Each train station’s physical coordinates was used as the merging point for the geospatial datasets.

## Algorithms:
Aggregated the Number of Entries and Exists from cumulatively tracked data. 
If the final aggregation exceeded 1000 for Dec2020-Mar2021 data, and 4500 for Dec2018-Mar2021 data, then they were dropped.
After reviewing every many cases in each dataset’s .99 quartile, these numbers were set as the threshold for data entry errors.
Further aggregations were done on specific column levels using groupby functions.

## Tools
Pandas for data manipulation,
Numpy matplotlib and seaborn for plotting,
Geopandas for Geospatial analysis,
SQLLite for database,
Sqlalchemy
