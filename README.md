We have a dictionary and want to convert it into a feature matrix, By default DictVectorizer outputs a sparse matrix that only stores elements with a value other than 0.
This can be very helpful when we have massive matrices (often encountered in natural language
processing) and want to minimize the memory requirements. We can force DictVectorizer to output a
dense matrix using sparse=False.
We can get the names of each generated feature using the get_feature_names method, While not necessary, for the sake of illustration we can create a pandas DataFrame to view the output
better, A dictionary is a popular data structure used by many programming languages; however, machine
learning algorithms expect the data to be in the form of a matrix. We can accomplish this using scikitlearn’s DictVectorizer.
This is a common situation when working with natural language processing. For example, we might
have a collection of documents and for each document we have a dictionary containing the number of
times every word appears in the document. Using DictVectorizer, we can easily create a feature
matrix where every feature is the number of times a word appears in each document In our toy example there are only three unique words (Red, Yellow, Blue) so there are only three
features in our matrix; however, you can imagine that if each document was actually a book in a
university library our feature matrix would be very large (and then we would want to set spare to
True)
