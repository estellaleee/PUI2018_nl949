# Idea
this is not really the idea. it is between and idea/theory and a null hypothesis. Describe the idea without worrying about defining the exact time frame, and justify why it is interesting/motivate it.

# Null hypothesis
This is the same as your idea, which is wrong: the null hypothesis should be the opposite. If you want to prove women bike less at night you should set up to disprove the opposite, i.e. that mand bike *less or the same* in that time frame, not more

# Formula
Missing!

If you tried to write a dormula you would have found out that you were missing a piece of the night time definition: 8PM till when?


# Data
The data processing *does not* support the idea, as I do not see where you remove the daytime rides and are left with 
"after 8PM". 

Then you need to throw away the weekdays

Thjen you need to creaste the 4 groups to compare:
men day, women day, men night, women night.


# Test

this will end up as a test of proportions or a test of means.

if this is a difference between means of samples, so the t test would work. however the distributions are not Gaussian. the t-test assumes Gaussianity and your distributions are not Gaussian. a non parametric test for difference of means is the Mann-Whitney U test (https://www.healthknowledge.org.uk/public-health-textbook/research-methods/1b-statistical-methods/parametric-nonparametric-tests) since the samples is large, the t-test may be ok
here is a list of assumptions the t-test makes https://www.investopedia.com/ask/answers/073115/what-assumptions-are-made-when-conducting-ttest.asp

if this is a test for proportions: a chi sq test would be appropriate and better than a Z test, since the Z test assumes gaussianity while the chi sq test is non-parametric

https://www.r-bloggers.com/comparison-of-two-proportions-parametric-z-test-and-non-parametric-chi-squared-methods/


