
## GOAL
Fit a model that explains variation in drug-related deaths in these counties in 2016. For simplicity, a linear model is recommended. 
Response variable will be the rate of drug-related deaths per 100,000 population (the standard way to measure this.) 
We'll take the counties as our units, so there's no need to weight the model by population.

## DATA
The file rustdrugs2016.txt contains county-level data on 2016 deaths from drug-related causes in the East North Central region, consisting of the states Ohio, Michigan, Indiana, Illinois, and Wisconsin.
The region is sometimes called the Great Lakes (although this usually includes Minnesota) or the Rust Belt (this usually includes Pennsylvania.) 

The variables are:
- County
- Deaths: number of drug-related deaths in 2016
- Population in 2016
- Area: land area of county in square miles
- PctWhite and PctBlack: percentage of the population who are white and black respectively
- Income: median household income
- Trump: proportion of 2016 Presidential election votes that went to Trump
- Obama: proportion of 2012 Presidential election votes that went to Obama


Question

1. Draw  pairs plot of data and comment on potential problems with model-building (outliers, extreme skewness, multicollinearity), or say "it's all good" if there are no such problems.

2. We wish to determine whether our model requires an income:Trump interaction. Draw sets of one-way and two-way faceted plots to graphically examine this potential interaction. Explain what plots tell about the need for this interaction in the model.

3. Fit a model to explain the drug death rate in these counties.  Display the model fit graphically in a way that emphasizes the interaction.

Please read the report for details.
