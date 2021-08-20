# House-prices-prediction

## 01 EDA

### Features
![Alt text](plots/SalePrice_histplot.png?raw=true "Histplot for dependent variable ('SalePrice')")

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