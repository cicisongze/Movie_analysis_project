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
When analyzing the data, we first extract the [Season] attribute from [Release date], and then separate the strings in [Genre] to build a word cloud. Further, we convert the [Runtime] to minutes applying the datetime package, and convert values in other columns to its correct type. 

Firstly, we yield the basic stats info as well as the pdf of numerical attributes, then by grouping them together, we get the relationship between each attributes. We also draw the best-fit lines, heatmap and and 3D-graph of these attributes. We found that, similar to our hypothesis, BoxOffice is positively related to budget, revenue, and 

## Instructions:





