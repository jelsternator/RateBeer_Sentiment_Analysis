# Beer Sentiment Analysis in Python
Scope consists of three parts:

1. Scraping Reviews/Ratings from RateBeer.com into Pandas Dataframe
2. Perform Cursory EDA/Visualiztion on DataFrame to guide next steps
3. Run Sentiment Analysis on review data to determine whether positive/negative ratings can be determined

----------------


## Part 1: Scraping Data using BeautifulSoup and Pandas
RateBeer.com has a top 50 list (https://www.ratebeer.com/top) that we will use

Steps:

1. Create dataframe containing all top level beer information: 'Rank', 'Name', 'Type','Reviews','ABV', 'Score'

2. Iterate over list of URLs to add Beer specific information: 'Brewery', 'City', 'State', 'Description'

3. Iterate over list of URLs to create Python dict/Pandas Dataframe of reviews and ratings for each beer
(Note: Review text scraping done later in notebook)

----------------

## Part 2: Perform Cursory EDA/Visualization using Matplotlib and Seaborn
Steps:

1. Check for normality of different data sets (Reviews/beer, ABV/Beer, Ratings/Beer)

2. Check for correlations between statistics (eg: ABV vs Rating, ABV vs State)

3. Getting overview of other summary statistics to investigate any points of interest

--------

## Part 3: Performing Sentiment Analysis using NLTK and TextBlob
Steps:

TOKENIZE/WORD FREQ/CREATE MODEL AND TEST IF HIGHER POS LEADS TO HIGHER RATING

1. Scrape all text of reviews into Python dictionaries

2. Tokenize all words to determine word frequencies

3. Define Positive and Negative reviews to train classification model

4. Test model to determine whether sentiment is correlated with overall rating


_______

### Notes:
Outputted files have been added to the repo to speed up timing of exercise, but they can be reinitialized/overwritten at any point with updated data as reviews/ratings are added and beers rise/fall in/out of the Top 50 list
