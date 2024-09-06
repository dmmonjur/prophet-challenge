# prophet-challenge

**Project Overview**

You are tasked with analyzing the Google search traffic and stock price data for MercadoLibre, the most popular e-commerce site in Latin America. The goal of this analysis is to identify patterns in search traffic and investigate any potential relationship with stock price movements. The steps are divided into four main sections:

Find Unusual Patterns in Google Search Traffic
    Mine the Search Traffic Data for Seasonality
    Relate Search Traffic to Stock Price Patterns
    Create a Time Series Model using Prophet

**This project is aimed at providing insight into how user interest, as reflected by search traffic, can be used to make informed decisions about stock trading.
Files in Repository**

Jupyter Notebook (prophet_challenge.ipynb): Contains all code for reading and analyzing the data, and generating the time series model.
    mercado_stock_price.csv: Dataset with MercadoLibre's stock price data.
    mercado_google_search_trends.csv: Dataset with Google search trends data related to MercadoLibre.

## How to Use This Repository

1. **Clone the Repository**
   ```bash
   git clone https://github.com/dmmonjur/prophet-challenge.git


2. **Install Dependencies**
   ```bash
  

    pandas
    matplotlib
    seaborn
    Prophet (for time series analysis)
   pip install pandas matplotlib seaborn prophet


3. **Run the Analysis Open the Jupyter Notebook (athletic_sales_analysis.ipynb) and run the cells to perform the analysis.**



## Aanalysys:
**Step 1: Find Unusual Patterns in Hourly Google Search Traffic**

Load the search trends dataset into a DataFrame.
    Slice the data to May 2020 and visualize the search trends for that month.
    Calculate the total search traffic for May 2020 and compare it to the median traffic across other months.
    Analyze any unusual patterns linked to MercadoLibre's financial results released in May 2020.

**Step 2: Mine the Search Traffic Data for Seasonality**

Analyze hourly, daily, and weekly search patterns to identify any predictable traffic trends.
    Group the data by:
        Hour of the day
        Day of the week
        Week of the year
    Identify trends such as peak times for user activity or seasonality in traffic, such as increased interest during holiday periods.

**Step 3: Relate Search Traffic to Stock Price Patterns**

Load and plot the stock price data for MercadoLibre.
    Concatenate stock price data with search traffic data for analysis.
    Investigate trends from January to June 2020 to see if the two time series follow similar trends during market events.
    Create new features in the DataFrame:
        Lagged Search Trends (1-hour shift of search data)
        Stock Volatility (4-hour rolling window standard deviation)
        Hourly Stock Return (percentage change in stock price)
    Calculate the correlation between search traffic, stock volatility, and stock returns.

**Step 4: Create a Time Series Model with Prophet**

Prepare the search trends data for time series forecasting using Prophet.
    Fit the Prophet model to predict future search traffic.
    Plot the near-term forecast of MercadoLibre's search traffic.
    Visualize the components of the forecast to answer questions about:
        Peak hours for search traffic
        Days of the week with the highest traffic
        Lowest point of search traffic in the calendar year

## Key Insights

The analysis reveals significant trends in search traffic during specific times and market events.
By leveraging search traffic data, it may be possible to predict stock market movements and make strategic investment decisions.
The time series forecast helps identify patterns in user interest throughout the day, week, and year, offering opportunities to optimize marketing efforts.

## Conclusion

This project demonstrates how search traffic data can be analyzed and used to forecast potential stock market trends, providing actionable insights to help MercadoLibre grow.
