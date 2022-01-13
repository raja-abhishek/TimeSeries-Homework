# TimeSeries-Homework

### Background
With over 200 million users, MercadoLibre is the most popular e-commerce site in Latin America. Task is to analyze the company's financial and user data in clever ways to make the company grow. So, main objective is to find out if the ability to predict search traffic can translate into the ability to successfully trade the stock.

### Analysis Steps:
- Step 1: Find unusual patterns in hourly Google search traffic
- Step 2: Mine the search traffic data for seasonality
- Step 3: Relate the search traffic to stock price patterns
- Step 4: Create a time series model with Prophet
- Step 5 (optional): Forecast revenue by using time series models

### Summary of the findings and Model

- Hourly Google search traffic data between Jun 2016 and Sep 2020 was analyzed which shows that search traffic in May'20 is 8.5% higher compared to the monhtly median search traffic across all months
- Search trafiic seasonality 
  - Search traffic is high on weekdays compared to weekends
  - Irrespective of the day of the week, serach traffic is high around the midnight
  ![alt text](http://url/to/img.png)
- Relation between search traffic and stock price pattern
  - A correlation analysis between lagged search traffic, stock volatility and hourly change in stock price shows that there is no predictable relation exist between all three series
- Time series model to prdict the search traffic
  - A time series model was developed using FB Prophet and Google search data to predict the search traffic
  - Component of the model shows that
    - Search traffic peaks on Tuesday and goes down for rest of the week
    - Search traffic is at lowest level Between September and November
    - Serach traffic is at highest level around the midnight
  - Search traffic trend shows it is declining and thats why near term forecast shows a decrease in search traffic
- Time series model to prdict the revenue
  - A time series model was developed using FB Prophet and historical revenue data to predict the next quarter sales
  - Component of the model shows that
    - Revenue is trending higher
    - First three days of the week (Monday, Tuesday and Wednesday) are the high revenue days
  - Forecasted Q3 2020 Sales (numbers are in USD, million):
    - Expected total sales - 2163.61
    - Best case scenario sales - 2337.90
    - Worst case scenario sales - 1988.68

