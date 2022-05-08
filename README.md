# Refactor VBA Code and Measure Performance

## Overview of Project

### Purpose

This project constructs a VBA program for analyzing stock data, compiling the starting price, ending price, and total trading volumes for 12 green energy stocks. The analysis was conducted on a data set with 6,000 daily price observations on the 12 stocks for the years 2017-2018. The VBA program was tested on this small data set, then refactored to be able to run on larger datasets.

## Analysis and Challenges

### Analysis of Stock Data

The dataset contained daily information on 12 stocks for the calendar years of 2017 and 2018; data fields included the stock ticker, date, opening price, closing price, adjusted closing price, daily high & low prices, and daily trading volume. 

VBA scripts were written to create several new variables, including total trading annual trading volumes, annual starting and ending prices, and annual return (i.e., difference between the starting and ending price for the year) on each stock. These new variables were compiled in tables included in the results section below.

### Challenges and Difficulties Encountered

The refactoring step included creation of a numeric stock ticker index to replace the use of individual stock tickers for compiling results. I was unable to make this index work properly when trying to loop through the data arrays, so the final VBA script "AllStocksAnalysisRefactored" fails to extract the annual reporting data after the first stock. The first VBA script "yearValueAnalysis" works properly, providing correct annual reports for all stocks, formatted and color coded for ease of use.

## Results

- Results for 2017. This was an excellent year for green energy; the 12 stocks averaged returns of 67%, ranging from a low of -7% to a high of +199%.

https://github.com/benniehana111/stock-analysis/blob/main/Resources/2017%20stock%20analysis.png

- Results for 2018. The green energy market turned sharply downward in 2018; the 12 stocks averaged returns of -8.5%, ranging from a low of 63% to a high of +84%.

https://github.com/benniehana111/stock-analysis/blob/main/Resources/2018%20stock%20analysis.png.

- Advantages and disadvantages of refactoring code in general.

Refactoring code offers the potential advantage of reducing coding steps, coding errors, required computational time and resources, and improved readability. The principal disadvantage are the extra programming time required, and the potential for new errors to be introduced.

- Advantages and disadvantages of the original and refactored VBA script.

The original VBA script performed as required with no errors. The refactored script should be capable of performing faster on large datasets, but I was unable to get the more advanced programming loop to work in the allotted time.


