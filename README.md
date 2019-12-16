# Thematic Analysis of Album Lyrics

## Navigating the Repo
Our main code can be found in the Project Pipeline.ipynb file. In order to run our code, make sure to extract the 380000-lyrics-from-metrolyrics.zip file to obtain the lyrics.csv file, which is used in our code to obtain the data from the dataset. The visualizations folder contains the .png files of our visualizations, but these visualizations can also be seen in the notebook itself. The lda_tuning_results.csv contains all intermediate results of the grid search we used to optimize our parameters. 

## Abstract
The aim of the project is to evaluate to what extent are a musical artist’s work reflective of their cultural world. More specifically, we intend to conduct topic analyses on the lyrics of well-established artists with considerably large discographies. These artists include Pink Floyd, David Bowie, Black Sabbath, Joy Division, and Metallica. The artists that were picked published music in similar timeframes, so that it is easier to draw a correlation between the results of each discography. Each artist was also selectively chosen because of their distinct background genre blends. Even when Black Sabbath and Metallica are both metal bands, they still differ in their respective subgenres. The relevance and motivation of this project lies comfortably in the disciple of cultural studies; i.e. to see if there is any within-period, cross-genre similarity between artist’s lyrics. If any similarity is found, we will try to link this similarity to historical events belonging to the common knowledge sphere of their respective time periods, to see if there is any relationship between an artist’s lyrics and their socio-cultural environment at the time of release.

## Research questions
A list of research questions you would like to address during the project:
- Is there any within-period, cross-genre similarity between artists’ lyrics?
- To what extent do lyrics from different time periods share similar content?
- To what extent do lyrics from varying musical genres share similar content?
- Is there a relationship between an artist’s lyrics and their socio-cultural environment at the time of release?


## Dataset
For this project we need data containing the lyrics of at least some of the songs pertaining to each album of each artist in the period into consideration (1970-1980), and metadata on the artist, the name of the song and, hopefully, the date of publication of the song.
Useful datasets containing song lyrics and some metadata are the following:

- https://www.kaggle.com/gyani95/380000-lyrics-from-metrolyrics
- https://www.kaggle.com/mousehead/songlyrics

We have not been able to check whether the artists we want to are in there, but we believe that they most probably are.

The datasets are on average 250000 lines, of which each one contains the text of the whole song. We are concerned that importing these databases in our laptops might be heavy on the memory, at least until we filter out all the songs we do not want to consider. Hopefully, the format of the lyrics is a string with a decently normal encoding.

We will process the lyrics string using the standard Natural Language Processing pipeline.


## A tentative list of milestones for the project

Add here a sketch of your planning for the coming weeks. Please mention who does what.

*Milestones*  
Week 1:  
- Translate datasets to a usable format, see if there is enough data on the selected artist, if necessary, decide on new artists - Jaël
- Filter selected artists out of datasets, clean data if necessary - Ludovica
- Develop natural language processing pipeline (tokenize sentences, lemmatize and normalize) - Jaël  

Week 2:  
- Clustering & topic modeling (https://www.machinelearningplus.com/nlp/topic-modeling-gensim-python/) - Ludovica  

Week 3:  
- Visualization of results using Matplotlib - António
- Results analysis - Jaël, António, Ludovica  

Week 4:  
- Documentation - Jaël, António, Ludovica  

Week 5:  
- Presentation - Jaël, António, Ludovica


## Documentation
This can be added as the project unfolds. You should describe, in particular, what your repo contains and how to reproduce your results.

## Sources
A preliminary list of sources we would like to use:

Implementations of topic analysis of lyrics:
- https://www.kaggle.com/devisangeetha/sing-a-song-lyrics-is-here/
- https://www.datacamp.com/community/tutorials/R-nlp-machine-learning
- https://www.kaggle.com/rtatman/nlp-in-r-topic-modelling

Some nice analyses of lyrics:
- http://dataffiti.com/2016/01/17/analyzing-rap-lyrics-part-1-of-3-creating-a-corpus/
- https://michaeljohns.github.io/lyrics-lab/
- https://towardsdatascience.com/sing-song-with-text-mining-cd8508ab51a5

A nice explanation of topic modeling:
- https://www.tidytextmining.com/topicmodeling.html
