# Overview
The Markov chains have been widely applied in multiple areas from physics, engineering and biology to marketing and finance (Norris, 1997; Privault, 2013). This repository is exclusively focused on the transition matrices whose probabilities are expressed in percentage (Privault, 2013). To showcase this particular application of Markov Chains, the Fortune Global 500 list on the world's largest companies was scraped and prepared. Specifically, the compiled dataset covers lists of the previous four years (from 2020 to 2023). A 4-year transition matrix based on the companies' profit was computed and styled using Python.

# About the method
## 1. Calculation of profit classes
Profit classes are the resulting categories of the calculation which splits up the profit from the Fortune Global 500 companies into 10 equal parts based on the cumulative percentage.

The calculation is as follows:
+ To sort the companies in descending order according to its profit;
+ To assign the profit classes from 1 to 10 in line with the respective cumulative percentage;
+ Figures <=0 are excluded from the calculation and categorized as "<=0".
<br>

**Image 1: Profit classes calculation**
<br>
![](https://github.com/IvoDSBarros/transition-matrices/blob/35e7e9784bce96f5a58de1114c148efc72294435/output/png/transition_matrices_calculation_support.PNG)


## 2. Interpretation of the transition matrix
+ The probabilities of the transition matrix are expressed in percentage, as stated previously;
+ The columns represent the profit classes of a later year of the time range (2023 in this case), whereas the rows represent the profit classes of a previous year (2020);
+ A color coding method was adopted to identify the different types of transitions;
+ Green segment (lower triangular): it portrays positive transitions in the matrix meaning any transition from a lower class of a previous year to an upper class of a later year; steep positive transitions are highlighted in dark green and, on the other hand, intermediate and slight positive transitions are highlighted in light green;
+ Yellow segment (diagonal): same profit class in both years of the analysis;
+ Red segment (upper triangular): it portrays positive transitions in the matrix meaning any transition from a lower class of a previous year to an upper class of a later year; steep positive transitions are highlighted in dark green and, on the other hand, intermediate and slight positive transitions are highlighted in light green.
<br>

**Image 2: 4-Year Profit transition matrix on the Fortune Global 500**
<br>

![](https://github.com/IvoDSBarros/transition-matrices/blob/9c568ccbc3c743a67c7de10a21c09064f50f45c4/output/png/transition_matrices_4_year_profit_tm.PNG)
