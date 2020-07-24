# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Project 3: r/python vs. r/Golang

## Table of Content:

1. [Executive Summary](#Executive_Summary)
1. [Description of Data](#dod)
1. [Findings](#find)
1. [Next Steps](#next)

## Jupyter Notebooks:
- [API and Data Gathering](API_and_Data_Gathering.ipynb)
- [NLP](NLP.ipynb)
- [Modeling](Modeling.ipynb)
- [Visualization](Visualization.ipynb)

## Executive Summary<a name="Executive_Summary"/>
1. Problem statement

Many new languages try to come for the champ, Python. One newcomer is Golang, a language developed at Google. Recently I've been reading a lot about people moving to Golang, and I've become interested in the differences between the users.  

To this end, I want to see what the differences are between r/python and r/Golang posts. I hypothesize that not only do the posts differ enough for model to accurately predict which subreddit a post originated from, but also that sentiment analysis can do the same.

2. Description of data:<a name="dod"/>

	Data size:
	 >Final Data shape is (2000x14)
	
	Data source:
	 >Source for [Reddit r/python, r/Golang data](./data/python1.csv)

	
	Data Dictionary:  
	
|Feature|Type|Description|  
|---|---|---|
***python***|int64|0, 1 for r/Golang or r/python post
***selftext***|object|text from the body of the post
***title***|object|text from the title of the post
***self_pol***|float64|selftext polarity score (-1 to 1)
***self_sub***|float64|selftext subjectivity score (0 to 1)
***title_pol***|float64|title polarity score (-1 to 1)
***title_sub***|float64|subjectivity score (0 to 1)
***title_words***|float64|title word count
***self_words***|float64|selftext word count
***words***|float64|total word count (self_words + title_words)
***sentences***|float64|total sentences count
***text_pol***|float64|text polarity score (-1 to 1)
***text_sub***|float64|text subjectivity score (0 to 1)
***text***|object|total text (selftext + title)


3. Findings:<a name="find"/>

	>My presentation can be found [here](./documents/presentation.pdf)

Using sentiment analysis, it appears that my hypothesis was incorrect and there is no discernible difference between the two subreddits with regard to sentiment. 

Additionally, while we can model with about a 85% accuracy rate on unseen data, this leverages very obvious words like 'python' and 'go'. Removing these words reduces the effectiveness of the model to about the baseline of 50%.

 
4. Next Steps:<a name='next'/>

- Remove code snippets etc. from the text.
- Pull the comments and run them through modeling as well.