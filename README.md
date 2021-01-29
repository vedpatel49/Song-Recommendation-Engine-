# Spotify-Recommendation-Engine

A content based recommendation engine was built using the Spotify Playlist (https://zenodo.org/record/2594557#.X8kZXM1KjtS) and tracks datasets (https://www.kaggle.com/yamaerenay/spotify-dataset-19212020-160k-tracks). 

Locality Sensitivity Hashing techniques were used to recommend songs/playlist to users. The recommendation engine was built using the PySpark API and trained on Spark clusters.
Bucket Randomized Projection from PySpark API was used to perform a neighbourhood search as euclidean distance were considered. See more about this algorithm here (https://spark.apache.org/docs/2.2.3/ml-features.html#bucketed-random-projection-for-euclidean-distance)

A more general study on locality sensitive hashing algorithms can be found on this really intutive article from Tyler Neylon. Please refer to this link (http://tylerneylon.com/a/lsh1/)

Three recommendation models were built based on different application
1) User Artist Recommendation - Recommending new artists to users
2) User Song Recommendation - Recommending new songs to users
3) Playlist Song Recommendation - Recommendaing new songs to existing playlists

Please refer to the python notebooks in the repository to know more about the models and their performance

