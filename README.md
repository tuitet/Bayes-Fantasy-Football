# Bayesian Inference of Fantasy Football Statistics 

## Summary

**Goal**: The goal of this project was to infer which underlying statistics best predict fantasy football player performance. More specifically, the goal of this analysis is to determine which and to what degree underlying variables contribute to total fantasy points scored during the 2019 season. The deviance information criterion (DIC) will guide which models best explain the relationship between these underlying variables and total fantasy points.

**Dataset**: The dataset is a combination of two sets of fantasy football statistics: Next Gen Stats and Pro Football Reference. The Next Gen Stats has advanced underlying statistics about football players from the 2019 season, while Pro Football Reference has Fantasy Points statistics.

**Approach**: Since the response variable (total fantasy points) is a continuous variable, and we want to see how these explanatory variables affect the response variable, Bayesian Linear Regression is a sensible model to use. Because football statistics differ between different player positions, our analysis will be repeated for three different player classes: Quarterbacks, Running Backs, and Receivers (Wide Receivers and Tight Ends).

**Results**: Below are the key underlying statistics for predicting a player’s fantasy football scoring output:
- For Quarterbacks, Passer Rating is a strong positive predictor of total fantasy points, while
Average Completed Air Yards is a weak positive predictor. Interceptions and Max Air Distance are weak negative predictors.
- For Running Backs, Expected Rushing Yards and Rush Yards Over Expected are weak positive
predictors of total fantasy points.
- For Receivers, Receptions and Percent Share of Intended Air Yards are strong positive predictors of total fantasy points.


## Key skills being practiced in this project include:

Pre-processing and merging data from multiple data sources:
- Scraping or downloading datasets from online sources
- Cleansing, aligning, and merging imported datasets

Bayesian inference on merged dataset:
- Performing variable selection using either simple methods or elastic net (with a threshold for keeping important variables) or Bayesian stochastic search variable selection (SSVS)
- Proposing linear regression models using a combination of likelihood function and informative and non-informative priors
- Performing Gibbs sampling on the models to understand the relationship between explanatory variables and response variable
- Comparing models using DIC

##
## The report is composed of the below files:
- Main PDF Written Report: Tim-Tuite-Bayes-Project-Report.pdf
- Quarterback Statistics Inference: Tim-Tuite-Bayes-Project-QB.Rmd
- Running Back Statistics Inference: Tim-Tuite-Bayes-Project-RB.Rmd
- Receiver Statistics Inference: Tim-Tuite-Bayes-Project-WR-TE.Rmd
- Next Gen Stats 2019 Passing Statistics: ngs_2019_passing.csv
- Next Gen Stats 2019 Rushing Statistics: ngs_2019_rushing.csv
- Next Gen Stats 2019 Receiving Statistics: ngs_2019_receiving.csv
