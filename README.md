# python-datascience

## Final Project (Data Science)

### Objective

The goal of this project was to analyze correlation between food intake and its impact on Covid-19 fatalities

*DataSource(kaggle): covid19-healthy-diet-dataset by Maria Ren* 

### Framing the dataset

The dataset contains 4 files with fat quantity, energy intake (kcal), food supply quantity (kg), and protein for different categories of food (calculated as percentage of total intake amount). The dataset also indcludes obesity and undernourished rate (as percentage of overall popuation) and COVID data - confirmed/deaths/recovered/active cases (in percentage of current population for each country) as of Janury 15, 2021.

I imported the datasets using pandas and added in continent data to each file.

### Structuring the dataframe

- Removed countries where 'Confirmed' COVID cases,'Undernourished' & 'Obesity' data is Not Available.
- Validated the % of columns added up to 100% for each dataframe
- Cleaned up 'Undernourished' column to remove strings so that it could be used for further analysis
- Categorized individual columns into various categories for further analysis and removed those individual columns


### Analysis

I focused on the correlation between various aggregated food sources and COVID fatalities by using correlation matrix and scatter plots. I also used a Kernel Density Estimation KDE chart to aid the data visulatization.

For more info on KDE: https://mathisonian.github.io/kde/

### Conclusion

The data analyses showed stronger positive correlation between Animal product based diet and COVID deaths as compared to a more plant-based or seafood-based diet.


### Next Steps

This analysis was more of an exercise in data structuring, visualizing and identifying patterns. The data is directionally indicative, however further rigourous statistcial analyses using more datapoints to determine other factors is worth exploring.