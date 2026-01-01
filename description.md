We are provided a training dataset consisting of three panels of household surveys that were conducted in different years. Each household responds to a variety of questions, and their responses are recorded. The household’s daily consumption per capita is also recorded. Weights were assigned to each household according to the number of people in the household and the degree to which the household is representative of the overall population. From the consumption values and the weights, the consumption distribution is computed and the poverty rate–the proportion of the population with a per capita consumption below a certain consumption level or poverty threshold–was calculated.
The household-level surveys have the following sets features, provided in train_hh_features.csv:

Identifiers & sampling information
The weights in the dataset are population-expanded weights, meaning that they reflect the probability of sampling times the number of members in the household. These are used to convert household-level survey data to accurate population-level estimates.
Welfare & expenditure information
Demographics & household composition
Education & employment
Housing & utilities
Geography
Food-consumption indicators (last 7 days)
In addition, the household-level consumption labels are provided in train_hh_gt.csv in dollars per day per capita.

The full data dictionary for the survey data is provided in feature_descriptions.csv and the values for certain coded indicators are provided in feature_value_descriptions.csv.

For your solution, you should predict the household-level consumption for each survey response in the test set in dollars per day per capita (2017 USD PPP).
