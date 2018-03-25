#Pacific Gas and Electric Energy Forecasting:


This work is dedicated on predicting aggregated energy consumption of different customer sectors.

Data is available from [here](https://pge-energydatarequest.com/public_datasets).

The work is dividied into two sections. 

- Data Cleaning, Manipulation, Visualization and  Modelling using XGBoost: performed using ``Python``

- Data Bayesian Modelling : performed using ``R``



### Data Explanation:

There are 40 csv files available, 20 for gas consumption and 20 for electricity consumption.
Data is available for all quarters for 5 years from 2013 to 2017. 

The columns are:

- ``ZipCode``: the location of the energy customer
- ``Month``: month of the year
- ``Year``: year of measurement
- ``CustomerClass``: categorical with four levels (1) residential, (2) commercial, (3) agricultural, and (4) industrial.
- ``Combined``: If zipcode is not large enough. It is categorical with two class, Yes and No. 
- ``TotalCustomers``: number of customers consuming energy in that zip code.
- ``TotalKwh``: total KWh used **available for electrical energy data**
- ``TotalThm``: total gas usage ** available for gas energy data**

## Detail of the data:

"Customer usage data, both for gas (therms) and electric (kWh) usage, is reported by ZIP code, by month, by year, and by the four customer types – residential, commercial, agricultural and industrial. The reports on this data are made available pursuant to California Public Utilities Commission Decision 14-05-016 (view the Decision here). Accordingly, the public datasets meet Commission Decision rules for public aggregation of data, as follows: a minimum of 100 Residential customers; a minimum of 15 Non-Residential customers, with no single Non-Residential customer accounting for more than 15% of the total consumption. If aggregation is not met, the consumption will be combined with a neighboring ZIP code until the aggregation requirements are met.

 

Recipients of the usage data are solely responsible for any use of the data. PG&E disclaims all warranties and representations, express or implied, of any kind regarding the reports and data, including the accuracy of the usage data or reports or their uses for any particular purpose.
Reports are published quarterly and are provided in machine readable format (CSV files) and contain 3 months of usage data that is through the end of the calendar quarter indicated in the file name.
Usage for Net Energy Metered customers is reported at their aggregate, monthly net values."