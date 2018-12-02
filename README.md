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
Initially, we extracted the movie data separately from three websites, IMDB, Rotten Tomatoes, and TMDB, to get the following attrubutes: [BoxOffice, Rating, Genre, Votes],[meter score, audience score],and [Budget, Revenue, Year, Runtime] respectively. After the web scraping process is done, we convert the lists or dictionaries with information into data frames and combined to yield a csv data file for future analysis. When processing the data frame, we applied pandas, numpy,and regex packages in order to convert the web text into more readable frames. After the dataset being structured, we reindexed the dataframe and extracted the needed colunns to build visualized models for analysis.

## Data Analysis:
When analyzing the data, we first 

## Instructions:





