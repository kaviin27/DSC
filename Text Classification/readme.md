                                                # Sentiment Analysis on Twitter data
 
Dataset:
  •	Sentiment140 dataset from Kaggle is used for this purpose. 
  •	2 columns – Polarity with values 0 – Negative, 4 – Positive and tweet column containing the text of the tweet. 
 
Data Wrangling: 
  •	The same steps as mentioned earlier were followed, using demoji and re libraries to clean the texts. 
 
Model Building: 
  •	Genism’s Doc2Vec is used to build the model. 
  •	This involves 1st transforming the data into Tagged Documents format that is used in Doc2Vec. We use an inbuilt method for this. 
  •	The entire corpus is split into train and test sets. 
  •	Doc2Vec is initialized and the training set is used, post that we use build_vocab to build a vocabulary from the training set. 
  •	We then convert the training and test data into vectors i.e texts to a matrix of numerical values. Using .infer_vector methodsover the model. 
  •	LogisticRegrssion model from sklearn learn is used to train a model and then using it to predict. 
