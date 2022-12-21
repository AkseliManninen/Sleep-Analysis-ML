# Sleep-Analysis-ML

# Project description

The project studies how sleep duration and quality change day-by-day, and how behavior during the previous day affects sleep. The sleep-related factors such as caffeine consumption, activity or stress could have a big impact on sleep. The objective of this project is to find patterns in sleep quality by examining relationshops between sleep and other factors.

# Description of the dataset

The dataset contains sleep-related information that was collected by Dana Diotte between the years 2014 – 2018. Data is Diotte’s personal data from the Sleep Cycle application form Northcube. The dataset was published on the website Kaggle.com.
There are in total 887 observations from different days. There are no observations from each day, but from those days that there are, the dataset is well-filled as there is not too much missing data. Ten variables were tracked: Start, End, Sleep quality, Time in bed, Wake up, Sleep Notes, Heart rate, and Activity. The dataset is in .csv format.

# Conclusions

In this project, the goal was to find patterns in sleep quality and use behavior and time-related features to predict sleep quality. When studying correlations, it turned out that coffee had only a small negative dependency on sleep quality whereas tea had a stronger association with sleep quality. Somewhat surprisingly, going late to bed, eating late and stress had little effect on sleep quality. Another surprising finding was that mean sleep quality was higher when the subject went late to bed. However, the subject went rarely late to sleep and there were fewer observations from such days which could have affected the results.

The subject's sleep quality was relatively similar during the other days except for Fridays. On Fridays, the subject had considerably higher sleep quality which could indicate that on Friday-Saturday nights the subject prioritizes sleep or has some other positive behavior that is not available in this dataset. When analyzing the subject’s sleep quality visually over a longer time, the sleep quality varied day by day and no patterns were detected.

Three machine learning models - linear regression, support vector regression with radial basis function kernel and support vector regression with polynomial kernel were used to predict sleep quality. Three feature sets were constructed using the wrapper method with linear regression and support vector regression. One of the feature sets had all features and the other two were subsets. Linear regression achieved the lowest mean squared error and score. However, all models performed poorly, which was somewhat expected as based on visual analysis of the plots, there were no clear dependencies between the sleep quality and the other variables.

In addition to weak predictions, the other challenges were that many observations needed to be discarded in the pre-processing due to missing values. For the same reason, the heart rate was pruned out which would have been interesting to include in the analysis. Finally, as the behavior of the subject had little effect on sleep, which is contradictory to personal experiences, common sense and the literature, it begs the question of how accurate the Sleep Cycle application's sleep quality scores are.

For future research, this dataset could be used to analyze how sleep affects behavior during the following day such as caffeine consumption or stress or how sleep affects mood. However, this dataset is sort of limiting, as there seems not to be that high dependency between the given variables. If different data was collected such as the number of coffee and tea cups drank and when they were drunk or how intensive workouts were and how late they were performed, there could be stronger dependencies to be found.
