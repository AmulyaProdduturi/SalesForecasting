# SalesForecasting of Retail clothing:

This project is done for the following purpose:

1. To predict the Sales of different product categories of a Retail clothing store based on previous sales data.
2. To minimize the revenue loss by advising them to invest stock accordingly.
3. It acts as an essential tool for business planning, marketing and decision making.


Dataset used:

Macro Economic data: Data provides details on GDP value, Unemployment rate,Commercial Bank Interest Rate on Credit Card Plans, Cotton Monthly Price, Cotton Monthly production, Cotton Exports etc

Weather data: Date provides the high, avg , low values of Temperature, Humidity, Visibility, Sea pressure, Wind speed. Data also has precipitation values for every day and  also the weather event of every day .

Holiday data: Data provides the list of holidays and type of holiday from the year 2009 to 2015.

Train data: Sales data for different product categories from the year 2009 to 2015.

Data Preprocessing:

1.Dropping Null values: We are dropping the rows with NA values as we take the mean of every month data and convert the whole data from daily to monthly data.

2.Replacing T value in Precip col with 0.001. 'T' in precipitation means that precipitation is less than 0.001. Hence we will replace the value with 0.001

3.Dropping column weather_event and date: As there are a lot of null values, and as our idea is to convert daily data to monthly data. weather_event and day columns are of no use
4.Aggregating Daily data to Monthly data
5.Dropping columns Advertising Expenses and Partyinpower(PIP) from macro economic data. Most of the values in Advertising Expenses are ?'s and column  Partyinpower(PIP) has only one value 'Democrats'


Techniques used:

1.Linear Regression

2.Decision Trees

3.Random forests

4.Gradient Boosting Regression

Error metrics to evaluate the performance of the model:

Root mean square error
Mean absolute percentage error

Enhancements made to improve the performance of the model:

Few attributes which are highly corelated are removed using Variance inflation factor and Feature Importance.
Then all the four techniques are applied on the new dataset.

