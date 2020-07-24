# Project 2: Ames, IA Housing prices


## Executive Summary
1. Problem statement

>As a member of a local real estate group in Iowa, we're interested in getting into the real estate market of Ames, IA and making investments. With this data, how well can we predict housing prices and what features increase the price of houses?

2. Description of data:

	Data size:
	 >Final Data shape is (2051x81)
	
	Data source:
	 >Source for [Ames, IA training data](./datasets/train.csv)
	
	 >Source for [Ames, IA testing data](./datasets/test.csv)
	
	Data Dictionary:
	> [Ames, IA Data Dictionary](AmesHousing.txt)

3. Findings:

	>My presentation can be found [here](presentation.pdf)

>  Using a linear regression model, we were able to get the RMSE to around 30,000. This means that the mean error of our model on a sample is ~30,000 dollars. Additionally, our best R2 score was about .8, which means that about 80% of the variability in price was explained by our choice of features. Interestingly enough, the model which attempted to use our known collinear features performed more poorly than the model which used all numerical columns. I am not sure why this is at this time. This is even more interesting because I later(just) realized at least two of those columns are the PID and ID columns which should have no correlation at all.

>  We found that some of the features which contribute heavily to price are:  
-Total liveable sqft  
-Overall quality  
-Basement sqft  
-Garage size

 
3. Recommendations:

>Recommendations:  
-If we want a larger return on our investments, buy houses where we can cheaply upgrade the sqft, or add a garage.  
-Work on more feature engineering to get an even better model.   
-Use more robust modeling, such as Lasso or Ridge Regression.  
