## Document Classification

Your task is to implement a document classifier using the [k-nearest neighbors algorithm](https://en.wikipedia.org/wiki/K-nearest_neighbors_algorithm).

## Tasks

* Download the [training and development datasets](../raw/master/src/vector_space_models/dat.tgz):
 * `AA*`: Amazon Appliances
 * `AB*`: Amazon Books
 * `BC*`: Broadcasting Conversations
 * `BN*`: Broadcasting News
 * `CT*`: Conversation Texts
 * `NW*`: Newswires
 * `WB*`: Web Blogs
* Create vector space models from the training data using: 
 * Bag-of-words.
 * Bag-of-words using [stop-words](../blob/master/src/vector_space_models/stop-words_english_6_en.txt).
 * TF-IDF.
* For each document in the development set, predict which genre it belongs to using the trained models. Experiment with both the [Euclidean distance](https://en.wikipedia.org/wiki/Euclidean_distance) and the [Cosine similarity](https://en.wikipedia.org/wiki/Cosine_similarity).
* Submit your code `hw3.py` and prediction results:
 * bow-euclidean.txt.
 * bow-euclidean-stopwords.txt.
 * bow-euclidean-tfidf.txt.
 * bow-cosine.txt.
 * bow-cosine-stopwords.txt.
 * bow-cosine-tfidf.txt.

## Extra Credit

Extra credits (upto 2 points) will be given to those who submit programs with exceptional results using more advanced techniques. Your programs must be original and cannot be copies of some existing systems.