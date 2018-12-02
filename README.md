# Movie_analysis_project

## Group 27
F4, section 2
## Description:
An analysis will be conducted on the correlation between movie rating and its other attributes. The data will be extracted and collected from mainstream movie websites. Eventually, a library where results are stored will be generated.
## Data sources:
```
IMDB
Rotten Tomatoes
TMDB
```
## Dependencies:
```
requests
bs4 
BeautifulSoup
pandas
numpy
re
seaborn
scipy
matplotlib
datetime
mpl_toolkits

```
## Installation:
Python 3.6.5 or higher
(pip install dependences above)

## Data Extraction & Pre-Processing:
Initially, we extracted movie data from three main movie resources websites, IMDB, Rotten Tomatoes, and TMDB,seperately, to get these following attrubutes: [BoxOffice, Rating, Genre, Votes],[meter score, audience score],and [Budget, Revenue, Year, Runtime] respectively. After the web scraping process, we converted the lists or dictionaries with information into data frames and combined them together to yield a csv data file for future analysis. When processing the data frame, we applied pandas, numpy,and regex packages in order to convert the web text into more readable frames. After the dataset being structured, we reindexed the dataframe and extracted the needed colunns to build visualized models for further analysis.

## Data Analysis:
When analyzing the data, we first extracted the [Season] attribute from [Release date], and then separated the strings in [Genre] to build a word cloud. Further, we converted the [Runtime] to minutes applying the datetime package, and converted values in other columns to its correct type. 

Firstly, we yielded the basic stats info as well as the pdf of numerical attributes, then by grouping them together, we got the relationship between each attributes. We also drew the best-fit lines of these attributes, and found that, similar to our hypothesis, BoxOffice is positively related to budget, revenue, and number of votes. We also went deep into the time series analysis. Interestly, we found that for all four attributes: budget, revenue, boxoffice and even runtime, while there's a small drop in 2016, we found an increasing trend overall. However, one thing out of our expectation is that the box office spread by seasons didn't vary a lot. There's indeed one movie with huge boxoffice bar in autumn, but we could consider this as an outlier.

Secondly, we generated a Genre Word Cloud and a bar graph based on each genre's occurrence. Among all 20 different movie genres, we can tell from the graph that in the past 5 years, Drama films played a dominant role in film market regarding to its amount, which is almost 1.7 times than the next genre, which is Comedy. Furthermore, we created a correlation heatmap using data on Runtime, Budget, Revenue, BoxOffice, Rating, Votes, Year. From the heatmap, we noticed that there is a strong postive correlation between a film's BoxOffice and its Budget(around 0.73) and also the number of votes(around 0.76), as expected. However, we noticed that the correlation between Rating and BoxOffice is only around 0.41, which indicates that the rating does not have a great impact on a film's box office, and we also noticed that the correlation between Budget and Rating is only around 0.39, which implies that having a large amount of budget does not ensure the quality of a film. 

Secondly, we generated a Genre Word Cloud and a bar graph based on each genre's occurrence. Among all 20 different movie genres, we can tell from the graph that in the past 5 years, Drama films played a dominant role in film market regarding to its amount, which is almost 1.7 times than the next genre, which is Comedy. Furthermore, we created a correlation heatmap using data on Runtime, Budget, Revenue, BoxOffice, Rating, Votes, Year. From the heatmap, we noticed that there is a strong postive correlation between a film's BoxOffice and its Budget(around 0.73) and also the number of votes(around 0.76), as expected. However, we noticed that the correlation between Rating and BoxOffice is only around 0.41, which indicates that the rating does not have a great impact on a film's box office, and we also noticed that the correlation between Budget and Rating is only around 0.39, which implies that having a large amount of budget does not ensure the quality of a film.

Next, we generated a fancy 3D-plot,and once again we confirmed that budget is not necessarily bounded to rating, while a high rating score does not guranteen a good return in box-office.


## Instructions:
Despite of all our graphing analysis, when running to the end of 'Data_Visualization', we implied a simple interface. Typing the specific year, genre, or score, you would find a list of recomended films. Clicking on the checkbox below, related graph will also be shown. 




