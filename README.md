# InClassAssignment_Kaggle_Titanic
Brianna Boston Kaggle Findings Titanic 

The dataset I worked on was the train.csv data set for the Titanic problem. 
In the dataset I created two python notebook files, one which cleans the dataset, and the other which tells my story. 
In the CleanTrain.csv I used mean imputation, and mode to fill in NaN values. Due to the number of missing values being almost equal to the number of rows found in the dataset, I thought it was best to use simplistic ways to guess what the null values could be. Is this the best way probably not. 
In the notebook called Titanic_Boston, I asked myself three questions:
1.	Are there more females than male passengers?
2.	What is the average fare cost between both genders, and what is the average age seen on this boat?
3.	As age increase does the price of the fare positively correlate or negatively correlate, is there any correlation between them at all?
Findings to Questions:
1.	Using .describe() on my two subset dataframes called dfemale and dfmale
a.	Count of Females = 314, Count of Males = 577
b.	We reject our assumption that there are more females than males on the Titanic, therefore they are more males seen on the titanic than females.
2.	Using .describe() on my two subset dataframes called dfemale and dfmale
a.	Average Age for Females: 28
b.	Average Fare for Females: 44.48
c.	Average Age for Male: 30
d.	Average Fare for Male: 25.52
3.	Using .corr() and creating a correlation matrix, and scatter plots
a.	We notice between the genders on the correlation matrixes there is negligible correlation between Age and Fare Price. 
b.	Correlation for Age and Fare when Gender is Female is:  .162
c.	Correlation for Age and Fare when Gender is Male is: .100
d.	The scatterplots show no linear (positive,negative) growth in increase of age with fare price for both male and female. By looking at our scatterplots we can assume we either do not have enough information, or there is no linear correlation between age and fare price of gender. If I were to plot a line, I believe it would fall flat on the scatterplots showing no growth in the information we currently have. We can notice some outliers on our Scatterplot as well that do not fit the general distribution of points.

From our findings we can conclude that there is no significant correlation on age, and fare between genders. The Titanic seems to have more male passengers than females, as well the average Fare price seems to be higher for females than males. This is interesting since we have more males, I would think that males would have a higher average than females fare price. This could be a miscalculation due to the data cleaning, however there were no records of missing values in Fare. The only columns I had missing values were in Age, Cabin, and Embarked. Cabin and Embarked would not affect our conclusion since we are looking at Age, Fare, and Sex. For Age I did mean imputation, which could result in some skewness of results. Maybe if I used some supervised algorithm to better approximate the results for correlation would be more significant? 

Citations:
https://towardsdatascience.com/eveything-you-need-to-know-about-interpreting-correlations-2c485841c0b8
https://datatofish.com/check-nan-pandas-dataframe/
https://www.analyticsvidhya.com/blog/2021/04/how-to-handle-missing-values-of-categorical-variables/
https://sparkbyexamples.com/pandas/pandas-convert-column-to-int/#:~:text=to%20int%20(Integer)-,Use%20pandas%20DataFrame.,int64%20%2C%20numpy.
https://towardsdatascience.com/converting-data-to-a-numeric-type-in-pandas-db9415caab0b
class textbooks
https://stackoverflow.com/questions/52657272/pandas-add-a-column-with-only-one-row
https://pandas.pydata.org/docs/reference/api/pandas.Index.html



 





![image](https://user-images.githubusercontent.com/93952383/198935849-810f82d3-4562-4383-a6a2-a44a0a00c163.png)
