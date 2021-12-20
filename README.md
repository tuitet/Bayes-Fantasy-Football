# bayes-fantasy-football
Bayesian prediction of fantasy football statistics 

In this project, we are predicting which players will perform best in a fantasy football season based on certain underlying statistics.  

The dataset we use is an amalgamation of two sets of statistics:  ”Next Gen Stats” powered by AWS andPro Football Reference. The Next Gen Stats has underlying statistics about football players from the 2019 season, while Pro Football Reference has Fantasy Points statistics.

The  goal  of  this  analysis  is  to  determine  which  and  to  what  degree  underlying  variables contribute to total fantasy points scored during the 2019 season. The deviance information criterion (DIC) will guide which models best explain the relationship between these underlying variables and total fantasy points.

Since the response variable (total fantasy points) is a continuous variable, and we want to see how these explanatory variables affect the response variable, Bayesian Linear Regression is a sensible model to use. Because football statistics differ between different player positions,our analysis will be repeated for three different player classes:  Quarterbacks, Running Backs, and Receivers (Wide Receivers and Tight Ends).
