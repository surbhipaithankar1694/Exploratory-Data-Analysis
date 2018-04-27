# Research question:
## To what extent do attitudes toward immigration explain the switching of votes of 2012 Obama supporters who became 2016 Trump supporters?

Polls have shown that people from certain demographic groups were more likely to switch their votes than others.
But what might explain why some people within a group switched, while others didn't?
One theory is that attitudes toward immigration became especially salient during the 2016 campaign.
This is useful but not really sufficient to study this problem, so we will explore the data and then fit a big and complicated logistic regression model.
We can't prove cause-and-effect from survey data (at least not with EDA), but we can get a sense of whether attitudes toward immigration had explanatory power over and above demographic shifts.

## Data  
We'll use the 2016 Cooperative Congressional Election Study, a very large survey of a nationally representative sample of 64,600 adults.  
The investigators asked questions to the sample both before and after the election, although not all the pre-election respondents replied to the post-election survey. 

Please read the report for detailed analysis.

Here are the variables we'll focus on.

### Technical variables:

commonweight_vv_post: The survey weights for people who took the post-election survey.
tookpost: Whether the respondent took the post-election survey. Limit your study to those for whom this is "Yes."
Demographic variables:

gender: Male or Female.
educ: Education (an ordered factor with six levels.)
race: A factor with eight levels.
pid7: Party identification (an ordered factor with seven levels from "Strong Democrat" to "Strong Republican.")
(One notable variable we omit is income, because the way it's coded in the CCES is hard to deal with.)

### Voting variables:

CC16_326: The respondent's vote in the 2012 Presidential election. Limit your study to those who voted for Barack Obama.
CC16_410a: The respondent's vote in the 2016 Presidential election. ``NA'' could mean they didn't vote or that they didn't take the post-election survey. Do not limit your study to those who voted for Donald Trump; otherwise you won't be able to give probabilities.
Immigration variables:

Respondents were asked: "What do you think the U.S. government should do about immigration? Select all that apply."

CC16_331_1: Grant legal status to all illegal immgrants who have held jobs and paid taxes for at least 3 years, and not been convicted of any felony crimes
CC16_331_2: Increase the number of border patrols on the U.S.-Mexican border
CC16_331_3: Grant legal status to people who were brought to the US illegal as children, but who have graduated from a U.S. high school
CC16_331_7: Identify and deport illegal immigrants
