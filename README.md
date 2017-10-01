# Text_intent_classification_Glove
Stanford's Glove word-vector embeddings are a representation of words into a n- dimensional (usually 300-D) vector hyperplane. Algorithms like n-grams are used to recognize the context in which a word comes. The algorithm chunks out group of n words from the sentence and then it tries to predict the neighbourhood words of the word under consideration. A shallow neural network gets trained through the loss gradually.
In this project, Stanford Glove's pre-trained model has been used as a reference for word-vectors of 400k words from wikipedia.
For intent classification of any sentence, each class is having some number of sample sentences,. All these sample sentences have been converted to certain vectors (by summing the vector values of individual words). The centroid of each class is calculated by taking the mean of vectors in each group.
Finally, the given sentence is converted to vector similarly and its distance from each centroid is calculated. The class with the minimum distance is the reqired class.

https://medium.com/rasa-blog/do-it-yourself-nlp-for-bot-developers-2e2da2817f3d
