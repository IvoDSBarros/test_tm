# Overview
The Markov chains have been widely applied in multiple areas from physics, engineering and biology to marketing and finance (Norris, 1997; Privault, 2013). This repository is exclusively focused on the transition matrices whose probabilities are expressed in percentage (Privault, 2013). To showcase this particular application of Markov Chains, the Fortune Global 500 list on the world's largest companies was scraped and prepared. Specifically, the compiled dataset consists of Fortune Global 500 lists of the previous four years (from 2020 to 2023). Several 4-year transition matrices based on the companies' profit were computed and styled using Python.

# About the method
## 1. Calculation of profit classes
Profit classes are the resulting categories of the calculation which splits up the profit from the Fortune Global 500 companies into 10 equal parts based on the cumulative percentage.

The calculation is as follows:
+ To sort the companies in descending order according to its profit;
+ To assign the profit classes from 1 to 10 as per the respective percentage;
+ Figures <0 are excluded and tagged as "<=0".
