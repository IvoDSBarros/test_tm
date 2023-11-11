# Overview
The Markov chains have been widely applied in multiple areas from physics, engineering and biology to marketing and finance (Norris, 1997; Privault, 2013). This repository is exclusively focused on the type of transition matrix of the Markov chain whose probabilities are expressed in percentage (Privault, 2013). To showcase this particular application of Markov chains, the Fortune Global 500 list on the world's largest companies was scraped and prepared. Specifically, the compiled dataset covers lists of the previous four years (from 2020 to 2023). A 4-year transition matrix based on the companies' profit was computed and styled using Python.

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

![](https://github.com/IvoDSBarros/transition-matrices/blob/97f8a15a69139ef69f0bc664ca925b3b1a73336b/output/png/transition_matrices_calculation_support.PNG)


## 2. Interpretation of the transition matrix
+ The probabilities of the transition matrix are expressed in percentage, as stated previously;
+ The columns represent the profit classes of a later year of the time range (2023 in the case in hand), whereas the rows stand for the profit classes of a previous year (2020);
+ A color coding method was adopted to identify the different types of transitions;
+ Green segment (lower triangular): it portrays upgrades in the matrix, meaning any transition from a lower class of a previous year to an upper class of a later year; steep upgrades are highlighted in dark green while intermediate and slight upgrades are marked in light green;
+ Yellow segment (diagonal): no ranking changes over the time period;
+ Red segment (upper triangular): red identifies downgrades (any transition from an upper class of a previous year to a lower class of a later year); the dark red intersections of the matrix are referring to steep downgrades and the light red ones are related to intermediate and slight downgrades;
+ Blue segment: companies which entered the Fortune Global 500 list;
+ Brown segment: companies which were dropped from the list.
<br>

**Image 2: 4-Year Profit transition matrix on the Fortune Global 500**
<br>

![](https://github.com/IvoDSBarros/transition-matrices/blob/9c568ccbc3c743a67c7de10a21c09064f50f45c4/output/png/transition_matrices_4_year_profit_tm.PNG)

<br>

**Image 3: 4-Year overall upgrade likelihood on the Fortune Global 500**
<br>

![](https://github.com/IvoDSBarros/transition-matrices/blob/c31b84a97c0eaa03b6eae0c8064905c86a61302e/output/png/transition_matrices_4_year_positive_transitions.PNG)

<br>

**Image 4: 4-Year overall downgrade likelihood on the Fortune Global 500**
<br>

![](https://github.com/IvoDSBarros/transition-matrices/blob/962ad4790be75cfe4ae14ac255ef40f0158ea6ee/output/png/transition_matrices_4_year_negative_transitions.PNG)


Find out more in the Jupyter Notebook.

# References
+ Norris, J.R. (1997) Markov Chains. Cambridge Series in Statistical and Probabilistic Mathematics. Series Number 2. Cambridge University Press. 237p. ISBN: 9780511810633.
+ Privault, N. (2013) Understanding Markov Chains. Examples and Applications. Springer Undergraduate Mathematics Series. 354p. ISBN 978-981-4451-50-5.
