# Predict future sales
## This is the final project for coursera online course: "How to Win a Data Science Competition: Learn from Top Kagglers". It is also a public challenge on the Kaggle platform. 
Reference: https://www.kaggle.com/c/competitive-data-science-predict-future-sales/overview 
Problem definition -
In this project, we would work with a time series data set consisting of daily sales data. The data is provided by the Russian software company “1C”. The training data consists date wise sales records categorized by shop id and item id. The task is to forecast the sales for next month (Nov-2015) for a shop id and item id combination.
There are about 6 million such records in the training set, collected over 30 shops selling 20,000 unique items. The training period is for 34 months starting from January 2013 to October 2015. Note that the train data set contains daily sales whereas we need to predict monthly sales for shop item pair in testing period. 
Data description -
    • sales_train.csv – The sales data from Jan-2013 to Oct-2015. 
    • test.csv – The project is to predict the sales for the shops and item pair for Nov-2015.
    • sample_submission.csv - a sample submission file. Note that it has an ID field that is unique representation of a (shop, item) pair.
    • items.csv – It contains information about an item’s category. 
    • item_categories.csv  - item_category_name field is not in English but contains a vital information about the item type and sub-type.
    • shops.csv- shop_name field contains a vital information about the city the respective shop belongs to.
Data fields -
    • ID – It represents a (shop, item) pair.
    • shop_id - Unique identifier of a shop.
    • item_id - Unique identifier of an item.
    • item_category_id - Unique identifier of item category.
    • item_cnt_day - Number of items sold. 
    • item_price - Current price of an item.
    • date – String in dd.mm.yyyy format.
    • date_block_num – Unique number for a month of a year. 
    • item_name – Item name. 
    • shop_name – Shop name.
    • item_category_name - Name of a item category.

Feature Engineering
    1. Extraction of City information from shop name.
    2. Extraction of item type and sub type from item category name.
    3. Various mean encoded sales lag features.
