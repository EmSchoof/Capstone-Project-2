## Context: MuseMe Music Genre Classification System
Music Genre Classification is one of the many branches of Music Information Retrieval, which encompasses beat tracking, music generation, recommender systems, track separation, and instrument recognition etc. Music analysis is a diverse field as each music session represents a distinct moment for the user, which makes describing and quantifying this moment an interesting challenge in the Data Science field.

The project  data sourced from a Kaggle page, "Spotify music genre list and 80k songs/tracks",  that contained over 131580 song instances  with 2800 music genres, and 80k extracted audio features.

## Goal: Distinguish between Music Genres based on Song Audio Features

#### Data Wrangling of songDB.tsv Kaggle Dataset
Natural Language Toolkit (nltk) was used to determine Music Genre Frequency Distribution in order to create a list of 20 root Genre Categories: 
- Alternative
- Electro
- Wop
- Reading
- Metal
- Chill
- House
- Indie
- Rave
- Cambinet
- HipHop
- Punk
- Rock
- Reggae
- Blues
- Pop
- Techno
- Dub
- Folk
- Jazz
A SQL query was then used to group each music genre within the sourced dataset in to it's respective Genre category.

#### Classification of Music Genres
- predict music genre by song audio features (data sourced from songDB.tsv)

**Conclusion for Music Genre Prediction**: The kNN classification model was successfully able to predict music genre based off of the audio features found in the dataset with 97.9% accuracy. However, it does seem odd that the ROC curve resulted in an equal ration of True(+) and False(+) rates.  

Further investigation into the procurement of the around audio features should be performed as their values and procurement were not heavily discussed in the Kaggle-sourced dataset. Until this is addressed, there is no way of determining if this model will accurately predict a music genre's by the same audio features if they are not recorded/converted/processed in the same manner. When sufficient proof has been made to support the claim that the audio feature extraction is repeatable, a less computationally dense classifier can replace the kNN model, such as SVM, Logistic Regression (Classification), or a combination in a neural network featuring several layers of classification and feature extraction as part of pipelined predictive model.

This model, when used in the manner described above, could be the music analyzer of a multi-dimensional music recommendation system that works in sync with additional datasets assessing how various users choose music genres.


## Acknowledgements
This work is a simplification from the Kaggle dataset posted at https://www.kaggle.com/grasslover/spotify-music-genre-list#songDb.tsv.
