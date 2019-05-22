# Trip Type Classification
- Kaggle: https://www.kaggle.com/c/walmart-recruiting-trip-type-classification
- Using gradient boosting(`LightGBM`)
- Key feature: **Upc > FinelineNumber > Department**

## Data Fields
- TripType - a categorical id representing the type of shopping trip the customer made. This is the ground truth that you are predicting. TripType_999 is an "other" category.
- VisitNumber - an id corresponding to a single trip by a single customer
- Weekday - the weekday of the trip
- Upc - the UPC number of the product purchased
- ScanCount - the number of the given item that was purchased. A negative value indicates a product return.
- DepartmentDescription - a high-level description of the item's department
- FinelineNumber - a more refined category for each of the products, created by Walmart


