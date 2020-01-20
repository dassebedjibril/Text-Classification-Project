# Text-Classification-Project
### Classification models for movie review data set.

For this project, we are going to be using a movie review data set and we are going to try to develop a classification 
model. However, we are going to be trying to predict simply based on the text of a movie review if that is `positive` or 
`negative` on the movie.

 We will start by importing the libraries:
 
`Import numpy as np`

`import pandas as pd`

For this project we'll use the Cornell University Movie Review polarity dataset v2.0 obtained from 

<a href='http://www.cs.cornell.edu/people/pabo/movie-review-data'>dataset</a>
and then we read the movie dataset with the following command `pd.read_csv('../TextFiles/moviereviews.tsv', sep='\t')`

In the dataset, 35 records show `NaN` (this stands for `not a number` and is equivalent to None). These are easily removed
using the `.dropna()` pandas function.

However, there are words in this list that may influence a classification of movie reviews. With this in mind, we will trim
the list to just 60 words and we’ll observe the accuracy changes. We explain the other steps throughout the project.


