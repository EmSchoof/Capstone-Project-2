## Context: MuseMe Music Genre Classification System
Music Genre Classification is one of the many branches of Music Information Retrieval, which encompasses beat tracking, music generation, recommender systems, track separation, and instrument recognition etc. Music analysis is a diverse field as each music session represents a distinct moment for the user, which makes describing and quanitiying this moment an interesting challenge in the Data Science field.

For the purpose of this study, these top 5 music genres will be used as classifers:
- RocknRoll
- Electronic
- Hiphop
- Indie
- Pop

## Goal: Distinguish between Music Genres based on Song Audio Features
#### Classification of Music Genres
- predict music genre by song audio features (data sourced from songDB.tsv)

**Conclusion for Music Genre Prediction**: The logistic regression model applied to the modified songDB.tsv dataset was successfully able to predict music genre based off of the audio features found in the dataset with 78% accuracy. Further investigation and modification of this model is necessary in order to prove if the audio features in this dataset are truly indicative of the song, to prove that audio feature extraction of the songs is can be consistently repeated, and finally, a neural network featuring several layers of classification and modification will further the accuracy of this model in order to create a real-time predictive model.


## Acknowledgements
This work is a simplification from the Kaggle dataset posted at https://www.kaggle.com/grasslover/spotify-music-genre-list#songDb.tsv and the work of The Echo Nest at http://the.echonest.com/.
