# House-prices-prediction

## 01 EDA

### Features
#### Dependent variable: SalePrice
![Alt text](plots/SalePrice_histplot.png?raw=true "Histplot for dependent variable ('SalePrice')")

We got 1460 sale prices with a mean of roughly 181K and a median of 163K. It is positively skewed. The maximum value is 755K and the minimum value is 35K. With a σ of 79K the values are fairly volatile. Lower and upper percentile are 130K and 755K respectively.

### Imputation
There's effectively only one missing value in the Electrical column, the rest can be relabeled according to the documentation. I chose to fill the one missing value with the mode of the column, i. e. `SBrkr` (Standard Circuit Breakers & Romex).

### Correlations
![Alt text](plots/corr_heatmap.png?raw=true "Correlation heatmap")

The features that correlate most with SalePrice are:
1. OverallQual - 0.79 (Rates the overall material and finish of the house)
2. GrLivArea - 0.71 (Above ground living area in square feet)
3. GarageCars - 0.64 (Size of garage in car capacity)
4. GarageArea - 0.62 (Size of garage in square feet)
5. TotalBsmtSF - 0.61 (Total square feet of basement area)
6. 1stFlrSF - 0.61 (First Floor square feet)
7. FullBath - 0.56 (Full bathrooms above grade)
8. TotRmsAbvGrd - 0.53 (Total rooms above grade)
9. YearBuilt - 0.52 (Original construction date)
10. YearRemodAdd - 0.51 (Remodel date)

![Alt text](plots/corr_heatmap_SalePrice.png?raw=true "Correlation heatmap - 'SalePrice'")

### Predictions
![Alt text](plots/prediction_plot.png?raw=true "Predictions")