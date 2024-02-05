# overview of population project

This data anlysis project aims to  Explore, analyze, and discover the intricate tapestry of global population dynamics 

## Table of contents
- [Data sources](#data-sources)
- [Tools](#tools)
- [Data Cleaning/ Preparation](#data-cleaning-preparation)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Results/ Findings](#results-findings)
- [Recommendations](#recommendations)


_
## Data sources
population_review_set : Downloaded from kaggle kernel (kaggle datasets download -d shiivvvaam/world-population-review-jan-2024)
## Tools
- Excel - Data store , Data Cleaning
- Python -Exploratory Data Analysis, Data preprocessing
- MySql - Data Analysis
- Tableau - creating reports and Dashboards



## Data Cleaning/ Preparation
In the data preparation phase, We performed these task
1. Data loading and inspection
2. Handling missing values
3. Data cleaning and formatting

## Exploratory Data Anlaysis 
- In the initial EDA phase, We performed four business moments
1. First business moment ( Measures of central tendency)
2. Second business moment ( Measures of dispersion)
3. Third business moment ( Skewness)
4. Fourth business moment ( Kurtosis)

## Data Analysis
```sql
 SELECT Area(km) AS mode_Area(km)
FROM (
SELECT Area(km), COUNT(*) AS frequency
FROM wpa
GROUP BY Area(km)
ORDER BY frequency DESC
LIMIT 1
) AS subquery;
```

## Results/ Findings
1.India hold a rank of no 1 in world population even though china is biggest nation in area than india it secures a 2 rank
2. but in the process of population growth rate, other coutries are in lead


## Limitations
 There were so many missing values, even though we imputed the missing values the data may not give meaningful insights as data is ordered according to population in desc


