# Evaluating Hashtag Activity based on Elon Musk’s Twitter History

### Team: Emily Parrish, M.S. Data Analytics
### Github Profile: https://github.com/emparrish417

#### Project Choice: (#3 Twitter Analysis) Leveraging one or more of the databases provided throughout the class, analyze the Elon-centric twitter dataset.

### Proposed Databases:
**Mongo**: Existing feature where hashtags are separated from the original text so it eliminates several pre-processing steps.

**Arango**: Networking and subgrouping based on hashtag content/behavior

## Project Description/Components:
The goal of this project is to assess the influence of Elon’s account activity on the account activity of his network.  This will be looked at primarily through hashtags both in content and frequency metrics.  Below lists some relevant sub-activities:

1.    Hashtag statistics and EDA: For the entire dataset, look at how often Elon and prominent figures in his network (aka the accounts that interact with him the most) are using hashtags at all and understand if there is a correlation between Elon’s hashtags and different rings of his network.

    - Query using mongo to pull all of the relavent hashtags.
    
    - Generate word clouds of hashtags (circle back on these when you have accounts grouped)
    
2.    **Ran out of time** Evaluate use of hashtags as a labelling technique:

    - Query tweet content only from mongo
    
    - Strip and lemmetize tweet content to prepare for topic modelling
    
    - Use NLTK to perform topic modelling 
    
    - Perfom side by side comparisons of the hastags from task one and the topics from the topic model...is there overlap?
    
    - Again do this for just Elon and then just his followers
    
3.   Identify subgroups based on hashtag activity and perform network analysis to potentially cluster these groups based on relationship with Elon (does he have a scientific/technology network, political network, etc.?)

    - Perform a graph traversal in arango to identify if certain hastags propagated from elon to followers. Use this information to develop subgroups.  Do members follow one another (aka double dependencies) or are they generally pulling these hashtags from Elon? Possibly a similar case with re-tweets.

### Additional Approaches:
1.    NLP techniques (i.e. topic modelling): use of automated unsupervised analysis techniques to compare actual content of tweets to hashtags.

    - Typically, MALLET (open-source) software package used for this. Also can use NLTK, which is more compatible with Python
    
    - Possibly use sentiment analysis libraries like Senti-Word NET to characterize Elon’s tweets in comparison with subgroups (would deviate from the hashtag focus)
