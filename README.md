# Trip Type Classification
- Kaggle: https://www.kaggle.com/c/walmart-recruiting-trip-type-classification
- Used gradient boosting(`XGBoost`)
- Key features: **Weight > Upc > FinelineNumber > Department**

## Data Fields
- TripType - a categorical id representing the type of shopping trip the customer made. This is the ground truth that you are predicting. TripType_999 is an "other" category.
- VisitNumber - an id corresponding to a single trip by a single customer
- Weekday - the weekday of the trip
- Upc - the UPC number of the product purchased
- ScanCount - the number of the given item that was purchased. A negative value indicates a product return.
- DepartmentDescription - a high-level description of the item's department
- FinelineNumber - a more refined category for each of the products, created by Walmart

## Key concept
### PFA: Principal Feature Analysis
- PFA is a kind of feature selection(http://www.ifp.illinois.edu/~qitian/e_paper/icip02/icip02.pdf)
- Use the weight of PC as coordinate for each original feature
- Implement K means Clustering and find centroid
- Calculate euclidean distance between each centroid and elements
- Select n feature which is close to each centroid

## Code
- `join_dataframe.ipynb`: overview a couple of dataframes to make train data set
- `make_dataframe.ipynb`: explain details how to create dataframes in `join_dataframe.ipynb`

