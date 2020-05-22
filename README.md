COMP6200 Data Science Portfolio 
===

Portfolio 1:

1. Analysis of CSV data for cycling strava and cheetah. Used inner join to join the two dataframes for which output will check the data on the index values. For data in strava if it is found in cheetah then the resultant dataframe will contain such entries. So the goal to keep only those rows of data that appear in both data frames so that we have complete data for every row is being statisfied by this type of join.
2. Since the date was being placed in the index 
3. Task 1 was to remove rides with no measured power (where device_watts is False). Checked for the unique values for device_watts field and found that there were Nan values also. Either the dataframe can be filtered by selecting just the true values or drop the rides with Nan values and select the filter out  false fields.
4. Task 2 was to look at the distributions of some key variables: time, distance, average speed, average power, TSS. Are they normally distributed? Skewed? I have used different ways to answer this question. First of all used subplot to plot two graphs of distance v/s TSS and distance v/s average_watts at a time. There appeared to be a linear relationship in both the plots. Used histogram to plot the time in seconds  for which there there was a right skewed histogram depicted. Created a dataframe indexes which contained the filtered out the joined_df for our varibales of interest.Skewness is the measure of asymmetry of the distribution. Applied skew() function to it. Now skew() is an in-built function we get the skewness of the data over a requested axis wherein a value closer to 0 represents a normal distribution.
5. Task 3 was to explore the relationships between the following variables. Are any of them corrolated with each other (do they vary together in a predictable way)? Can you explain any relationships you observe? For this purpose I have used a heatmap.  Heatmap is a rectangular color encoded matrix which shows the correlation between variables on a scale of 1 to -1. Correlation between the variables of our interest in indexes dataframe was found out. This correlation dataframe was used to generate the heatmap.
6. Task 4 was to find out if Races are more challenging than Rides in general? Firstly grouped the data on the 'workout_type' and applied median() to it, here we can compare the median NP values for different workout types. It is evident that Race is the highest as compared to others. Then splitted the joined_df for workout_type 'Race' and others two different dataframes. Heartrate is parameter which is very much related to a workout type hence was considered for comparision. The plot for the same reflected the assumption by having higher value for Average Heartrate in Races.
7. Task 5 was to generate a plot that summarises the number of km ridden each month over the period of the data. Made use of differnt plotting techniques for data visualisation. From the plot of month_df it looks like that the lowest activity was between May-2018 to September-2018.
8. This portofio was more about data visualisation. Data depending upon different features was to be represented to audience.

Portfolio 2:


