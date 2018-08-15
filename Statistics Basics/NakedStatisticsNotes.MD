# naked statistics

First off, before we start with the notes, here are some of my favorite __quotes__ from the book, all from Mr. Wheelan himself.

* *It’s easy to lie with statistics, but it’s hard to tell the truth without them.*
* *The greatest risks are never the ones you can see and measure, but the ones you can’t see and therefore can never measure. The ones that seem so far outside the boundary of normal probability that you can’t imagine they could happen in your lifetime—even though, of course, they do happen, more often than you care to realize.*
* *So it is with statistics; no amount of fancy analysis can make up for fundamentally flawed data. Hence the expression “garbage in, garbage out."* - this ones actually a prominent truth in artificial intelligence.


# Notes
Now that I have enlightened you with those memorable quotes, here's a small collection of notes to summarize some parts of what is said in the book.


## Statistical Software
* Excel
* R
* Stata
* SAS
* IBM SPSS


## Gini Index
* Statistical tool for collapsing complex info into a simple number
* Tool for comparison, no intrinsic meaning
* Ex: Wealth
  * Country where everyone has same wealth - index of 0
  * Country where one household has all the money - index of 1


## Statistics?
* Helps us process data
* Collection + analysis of data
* Generally for the purpose of planning experiments, summarizing them, etc.
* Quantitative / Qualitative data


## Sampling
* Process of gathering data for a small area, then using that data to make an informed decision / judgement / inference about the whole set of data.


## Scientific Method
* Says that if we are testing a hypothesis, we must conduct a controlled experiment with variable of interest being the only thing that differs between the experimental and control group


## Regression Analysis

The tool that enables researches to isolate a relationship between two variables while holding constant the effects of other important variables.
Estimates relationships between variables.

We use regression analysis to do two things:
* Quantify the association observed
* Quantify the likelihood that the association observed is a simple coincidence, and not representative of a greater trend

One of the drawbacks of regression analysis is that it can isolate a strong association between two variables through statistical analysis, but it cannot necessarily explain why the relationship exists.


## Descriptive Statistics
Descriptive statistics is a summary statistic. Ex:
* Batting average

Data aims to summarize a great deal of information into numbers. Since more data sometimes presents less clarity, we simplify it. We turn a huge collection of numbers into a single descriptive statistic, like a score.

For example, let's say that you just did a presentation. If the judges sat down and explained every single thing you did well and why, and things they disliked, that would take them substantially more time than if they summarized that 'data' about your performance into a single number - your score.

The __mean__ is not always accurate - outliers heavily influence the data. Hence, we also use __median__. If they are substantially different, that means that the data is littered with outliers. The closer they are, the more representative any one datum is of the whole dataset.

__Absolute Figures__ are numbers that can be represented without any context - temperature, etic

__Relative Figures__ are numbers that need proper context to be understood fully. For example, a score. If someone scored a 13/15 on a test, you don't know if its good or bad. However, if I was to tell you that they scored in the 90th percentile, that is much more descriptive - you know that they are in the top 10% of students. Most standardized tests produce relative figures, and need proper context to be understood.

__Standard Deviation__ is a measure of how dispersed the data is from the mean. The higher the deviation, the more dispersed the data.

__The Normal Distribution__ is a bell curve which tells us that in a dataset, the distribution of data will fall into the shape of a symmetrical bell curve, where 68.2% of the data is in +- 1 standard deviation from the median, 13.6% more on each side of that( two standard deviations from the median ), then 2.1 % of the data on each side of that ( three standard deviations from the median ), etc. This is best described in a [picture](http://www.statisticshowto.com/wp-content/uploads/2013/09/standard-normal-distribution.jpg).

The disadvantage of descriptive statistics is the same as its advantage - it consolidates its data into a single number. The index is highly sensitive to the descriptive statistics that are cobbled together to build it, and to the weight of each of those components. For example, if someone has a lower score on a test, it might be because they were sick, or came late, or for another reason; their score might be lower even if they are an extremely bright mind.

Descriptive statistics do not portray all sides of the data behind them, but provide a simple number that can be used to judge the data behind them *if used correctly*.


__Variance__ is calculated by determining how far the observations within a distribution lie from the mean. The formula can be found from a quick google.


## Description deception

__Precision__ reflects the exactitude with which we can express something - 41.654 miles is more precise than 'around 50'.

__Accuracy__ is a measure of whether a figure is broadly consistent with the truth. For example, if I was to say 'There are only 20 people on the earth' that would be a bald-faced lie, and hence not accurate.

However, if I was to say that there are '12.456 billion' people on the Earth, someone who has no knowledge of the population might believe me - my statement is inaccurate yet seems precise. That is an example that explains the distinction between the two.

Always pay attention to the unit of analysis. What/Who is being described, and is it the same across all reports / instances of that explanation?

__Nominal Figures__ are not adjusted for inflation, while __Real Figures__ are.

Always make sure that you are using the correct medium for displaying your data; this is to avoid statistical inaccuracy.


## Correlation

Measures the degree to which two phenomena are related. Two variables are positively correlated if a change in one is associated with a change in another in the same direction, negatively correlated if it is the opposite direction, and there is no correlation if change in one does not incur a change in the other.

Represented on a scale of -1 to 1.
* -1 is negative correlation.
* 0 is no meaningful association.
* 1 is positive correlation,

Correlation does not equal causation. For example, take a study where parents with more tv's tend to have brighter students. This is not because TV's make you intelligent - it is because families who tend to have more TV's are richer, and hence can finance their kids' education better than those with less money.


## Basic probability

Two independent events both happening - P(A) * P(B)

Probability of two mutually exclusive events happening is 0

Probability of two dependent events happening is P(A) * P(B|A)  - *Probability of A times probability of B given A has already occurred*


## Importance of Data

A data sample must be representative of some larger group, because inferences made from a reasonable large, properly drawn sample can be every bit as accurate as information gathered from the whole population. A properly drawn sample should look like the population from which it is drawn.

A bigger sample will not necessarily make up for bias or other errors in the data.

## Dataset types

Longitudinal study collects info on a large group of subjects at many different points in time over a long period of time - i.e. every 2 years for 30 years. These are the best types of datasets.

Cross-sectional data sets are collections of data gathered at a single point in time. These are not as good as Longitudinal datasets, but they are ok.


## Some Bias types

Self-election bias - when individuals volunteer for something

Publication bias - positive results are more likely to be published than negative results. This can skew the results which we see.

Recall Bias - memory is not always the best source of data, as it is fragile and easily influenceable.

Survivorship bias - when some or many of the observations are falling out of the sample, changing the composition of the observations that are left and therefore affecting the results of the analysis.

'Healthy User' bias - people who faithfully engage in activities that are good for them are fundamentally different from the rest of the population.

## Central Limit Theorem

A large properly drawn sample will resemble the population from which it is drawn. There will be some variance, but the probability that any randomly chosen sample will colossally deviate from the underlying population is quite low.
