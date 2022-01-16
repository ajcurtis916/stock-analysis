# Stock Analysis
## *Analyzing Stock Daily Volume & Annual Rate of Return*
### Purpose: Compare and contrast stock performance between 2017 and 2018, and refactor our code for maximum efficiency
---
## Results
## *Stock Performance Comparison Between 2017 & 2018*
<img align="left" src="https://github.com/ajcurtis916/stock-analysis/blob/main/resources/stock_performance_2017.png" width="250" />
2017 was a great year for all of the stocks.  Only one of the selected 12 stocks had a negative annual rate of return (AROR).  The highest performing stocks were DQ (199% AROR) and SEDG (184% AROR), closely followed behind by ENPH (130% AROR) and FSLR (101% AROR).  TERP performed the worst (-7% AROR).  Even though DQ performed the highest in 2017 based on AROR, DQ had the lowest total daily volume at 35,796,200.

<img align="right" src="https://github.com/ajcurtis916/stock-analysis/blob/main/resources/stock_performance_2018.png" width="250" />
In terms of AROR, most of the stocks took a fall in 2018.  All had a negative AROR except for RUN (84% AROR) and ENPH (82% AROR).  DQ performed the worst (63% AROR), closely followed behind by JKS (61% AROR).  Total daily volume had a wide range in 2017 and 2018.  Some stocks performed with a higher total daily volume in 2018 from 2017, and some performed with a lower total daily volume in 2018 from 2017.  It is worth noting that DQ had a higher total daily volume in 2018, up to 107,873,900 from 35,796,200 in 2017, but performed the worst out of any of the stocks in 2018.  ENPH appears the most promising for investment, as it performed very well in both 2017 and 2018, and had the highest total daily volume (607,473,500) out of all the selected stocks in 2018.</br></br>

## *Refactored Code Comparison*
<img align="left" src="https://github.com/ajcurtis916/stock-analysis/blob/main/resources/OG_code.png" width="550" />
Our original code and refactored code was identical for the first third, but divulged at the for loops and creation of output arrays in the refactored code that would later hold the values for total daily volume and annual rate of return (calculations involving the stock's starting and ending prices).  A tickerIndex variable was utilized in the refactored code to track which tickers and/or stock data attached to each ticker was being iterated through during the for loops and if-else conditionals.  The variable was then used to add values to the volume, starting, and ending prices, utilizing similar logic as the original code.  

<img align="right" src="https://github.com/ajcurtis916/stock-analysis/blob/main/resources/refactored_code.png" width="550" /></br></br>
The tickerIndex variable was again utilized in a for loop at the end of the subroutine for the final worksheet output.  The code for worksheet output in the original code was hardcoded.  This means the refactored code will be more beneficial if additional tickers are added in future years, after just a few code adjustments.</br></br>

In the refactored code, all formatting was included in the one subroutine, as opposed to separate subroutines in the original code.  As you may note in the pictures above, the refactored code included more lines of code.  As you will find below, even though the refactored code included more lines of code, it ran more efficiently.  The original code ran close to 3/4s of a second, while the refactored code ran close to 1/4 of a second.  In other words, the code efficiency increased by 300%.</br></br></br>

Original Code 2017     |  Refactored Code 2017    |    Original Code 2018     |  Refactored Code 2018  
:-------------------------:|:-------------------------:|:-------------------------:|:-------------------------:
<img src="https://github.com/ajcurtis916/stock-analysis/blob/main/resources/OG_run_time_2017.png" width="300" />|<img src="https://github.com/ajcurtis916/stock-analysis/blob/main/resources/refactored_run_time_2017.png" width="300"/>|<img src="https://github.com/ajcurtis916/stock-analysis/blob/main/resources/OG_run_time_2018.png" width="300"/>|<img src="https://github.com/ajcurtis916/stock-analysis/blob/main/resources/refactored_run_time_2018.png" width="300"/>

</br>

## Summary
Though the refactored code includes more lines of code, it runs approximatgely 300% more efficiently.  This means the refactored code is easier on the computer and it's memory.  If the code were to analyze a much larger database, this will be very beneficial.</br></br>
Since the refactored code utilizes the new tickerIndex variable in its for loops and conditionals, it will be much easier to adjust for different data such as adding additional stock tickers in the future.  Since the original code involved more hard coding, it would take a lot more time and effort for potential changes to future stock data.
