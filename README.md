# Walmart-Store-Sales-Forecasting

The dataset contains the historical data for 45 Walmart stores situated in different regions. Each stores contains numerous divisions or departments and the goal is to predict the sales for each department in each store. The dataset also include the selected holiday markdown events. These markdowns are known to influence sales, but it is challenging to anticipate which divisions are influenced and the degree of the affect. Walmart runs a few limited time markdown events throughout the year. These markdowns go before conspicuous occasions, the four biggest of which are the Super Bowl, Labor Day, Thanksgivings, and Christmas. The weeks counting these occasions are weighted five times in the evaluation than non-holiday weeks. Part of the challenge is modelling the impacts of markdowns on theses occasion weeks in the absence of complete/ideal historical data.


## Dataset

stores.csv: This file contains anonymized information about the 45 stores, indicating the type and size of store.

train.csv: This is the historical training data, which covers to 2010-02-05 to 2012-11-01. Within this file, you will find the following fields:

•	Store - the store number
•	Dept - the department number
•	Date - the week
•	Weekly_Sales -  sales for the given department in the given store
•	IsHoliday - whether the week is a special holiday week

test.csv: This file is identical to train.csv, except we have withheld the weekly sales. You must predict the sales for each triplet of store, department, and date in this file.

features.csv: This file contains additional data related to the store, department, and regional activity for the given dates. It contains the following fields:

•	Store - the store number
•	Date - the week
•	Temperature - average temperature in the region
•	Fuel_Price - cost of fuel in the region
•	MarkDown1-5 - anonymized data related to promotional markdowns that Walmart is running. MarkDown data is only available after Nov 2011, and is not available for all stores all the time. Any missing value is marked with an NA.
•	CPI - the consumer price index
•	Unemployment - the unemployment rate
•	IsHoliday - whether the week is a special holiday week
