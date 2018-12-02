## Analyzing Billboard Year-End Top 100 Singles from 1960-2017¶

The aim of the project is to analyze how popular music has changed since the 1960s and to predict if a song will be popular in future years based on its audio features. For the sake of this project, we have assumed a track is popular if it made to the Billboard Year End Hot 100 Singles. Billboard has been publishing a list of Hot 100 Singles since the 50s, we have scraped this list for each year from 1960 to 2017.
Spotify’s API endpoint get_audio_features provides some really interesting information about sound tracks such as loudness, instrumentalness energy, liveness, etc. Spotify API has been used to extract audio features of tracks, artist popularity, and track popularity on spotify.

Some of the questions our project aims to ask:
What makes the music today different from the music in 60s? the How has rise of certain genres and decline of others affected the audio features of music? What makes a song popular, are there certain audio features that are common to popular songs? If yes, can we predict if a song will make it to Billboard based on its audio features? What have popular musicians been singing about? Has the content of lyrics and primary message of tracks changed since the 1960s? How has average sentiment of song changed, are songs happier now than they were?

### 1. Scraping Billboard and Wikipedia to get Year End Hot 100 Singles:
The code for scraping Billboard and Wikipedia and getting audio features and Spotify can be found here.
https://github.com/Nayifff/ToolsProject/blob/master/BillboardHot100_WebScraping_InitialAnalysis_FINAL.ipynb

##### NOTE: This code takes several hours to run. Please start running this file from where the data is read into the notebook. We have saved the data extracted after scraping to 
https://github.com/Nayifff/ToolsProject/blob/master/spotify_project_final%20v2.0.xlsx


###	2. Topic Analysis on Lyrics Using Latent Dirichlet Allocation (LDA):
We used Topic Analysis algorithm LDA to understand how the content/message of top tracks has changed over the years. The code for this can be found here:  https://github.com/Nayifff/ToolsProject/blob/master/Lyrics_LDA_FInal.ipynb
The file used for LDA is: https://github.com/Nayifff/ToolsProject/blob/master/billboard_lyrics_1964-2015.csv

##### NOTE: Please run this code from the beginning


###	3. Sentiment Analysis on Lyrics Using Gensim:
Sentiment Analysis was conducted to understand the fluctuation in sentiments in tracks over the years. The code for this can be found here:
https://github.com/Nayifff/ToolsProject/blob/master/Lyrics%20Sentiment%20Analysis%20FINAL.ipynb
  
##### NOTE: Please run this code from the beginning



   
