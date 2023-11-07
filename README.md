# Overview
The Markov chains have been widely applied in multiple areas from physics, engineering and biology to marketing and finance (Norris, 1997; Privault, 2013). This repository is exclusively focused on the transition matrices whose probabilities are expressed in percentage (Privault, 2013). To showcase this particular application of Markov Chains, the Fortune Global 500 list on the world's largest companies was scraped and prepared. Specifically, the compiled dataset convers lists of the previous four years (from 2020 to 2023). A 4-year transition matrix based on the companies' profit was computed and styled using Python.

# About the method
## 1. Calculation of profit classes
Profit classes are the resulting categories of the calculation which splits up the profit from the Fortune Global 500 companies into 10 equal parts based on the cumulative percentage.

The calculation is as follows:
+ To sort the companies in descending order according to its profit;
+ To assign the profit classes from 1 to 10 in line with the respective cumulative percentage;
+ Figures <=0 are excluded from the calculation and categorized as "<=0".

![](https://github.com/IvoDSBarros/transition-matrices/blob/72d40d620791456479a64f206c8c34930ba3c223/output/png/transition_matrices_calculation_support.PNG)


## 2. Interpretation of the transition matrix
+ The probabilities of the transition matrix are expressed in percentage, as stated previously;
+ The columns stand for the profit classes of 2023, whereas the rows account for the profit classes of 2020.
+ The green segment 
