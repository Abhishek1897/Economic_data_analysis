# Economic Data Analysis Using FRED API

This project involves analyzing various economic indicators using the Federal Reserve Economic Data (FRED) API. The primary focus is on the S&P 500 index, unemployment rates, and labor force participation rates across different states. The analysis covers the period during the COVID-19 pandemic to understand its economic impact and the varying recovery patterns across states.

## Project Structure

### 1. Setup and Initialization
- Import necessary libraries: `pandas`, `numpy`, `matplotlib.pyplot`, `plotly.express`, `time`, and `fredapi`.
- Configure `matplotlib` style and `pandas` display options.
- Create the `Fred` object using the API key.

### 2. Search for Economic Data
- Perform a search for S&P data and obtain a DataFrame with information about different data series related to the S&P.

### 3. Raw Data and Plot
- Fetch the S&P 500 index data using `fred.get_series('SP500')`.
- Plot the historical performance of the S&P 500 index over time.

### 4. Pull and Join Multiple Data Series
- Search for unemployment data and filter it to find monthly, seasonally adjusted unemployment rates by state.
- Fetch the unemployment rate series for each state and combine them into a single DataFrame.
- Clean the combined DataFrame and plot the unemployment rates for all states using Plotly Express.

### 5. Pull April 2020 Unemployment Rate Per State
- Extract the unemployment rates for each state in May 2020 and plot them in a horizontal bar chart to highlight the unemployment impact during the peak of the COVID-19 pandemic.

### 6. Pull Participation Rate
- Perform a similar process for labor force participation rates, fetching data for each state and combining it into a single DataFrame.
- Rename the columns to reflect state names accurately.

### 7. Plot Unemployment vs Participation for Each State
- Create subplots for each state to compare unemployment and participation rates from 2020 to 2022.
- Plot specific states like California in more detail to showcase the trends in unemployment and participation rates.

## Insights

### S&P 500 Trends
- The S&P 500 index shows significant fluctuations over time, reflecting market conditions and economic events.

### Unemployment Rates
- The unemployment rates across states varied significantly during the pandemic, with some states experiencing much higher rates than others.

### Labor Force Participation
- The participation rate trends help understand the labor market's health and how active the workforce is in each state.

### State-Specific Trends
- By comparing unemployment and participation rates for specific states, we can gain insights into how different states managed their labor markets during the pandemic. For example, California showed noticeable changes in both metrics during 2020-2022.

## Conclusion
This analysis provides a comprehensive overview of economic indicators such as the S&P 500 index, unemployment rates, and labor force participation rates across different states. By examining these metrics, we can understand the economic impact of the COVID-19 pandemic and the varying recovery patterns across states. These insights can inform policymakers, economists, and investors about the labor market's dynamics and overall economic health.
