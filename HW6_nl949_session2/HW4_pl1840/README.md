###1a) Verify that null and alternative hypotheses are formulated correctly.
Their null hypothesis: "The time of subscribers biking are less than or equal to the time of non-subscribers spent on biking"
Their alternative hypothesis: "Subscribers spend more time biking per day than non-subscribers"

These seem to be formulated correctly! Good job. 

###1b) Verify that the data supports the project. Does the data have the appropriate features (variables) to answer the question? Was the data properly pre-processed to extract the needed values?

I generally try to avoid dropping columns in place, because it has always seemed to me to be more difficult to read exactly what the output is. I prefer to create new dataframes using .copy(), especially since it lets me go back to the original without having to re-import it if I've made a mistake somewhere (non-destructive method). 

This notebook gets to a dataframe with usertype and start-time, but doesn't seem to format the data into a place where they might then go and check ride duration, which they might consider calculating as ("ride_end"-"ride_start").astype('timedelta64[h]').

1c) Choose an appropriate test to test H0 given the type of data and the question asked.

We should use the chi-square test for homogeneity to test their hypothesis, since the question at hand concerns whether a potential difference in ride duration is associated with category of rider (subscriber vs. non-subscriber), or if any potential difference is due to pure chance. 