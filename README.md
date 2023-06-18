# BERT-Classification
Text classifcation of tweets regarding COVID using BERT pre-trained model.

# DATASET
 A covid dataset has been collected from kaggle.
 Using API calls, the dataset is directly accessed into Google Colab.
 The dataset contains of several parameters pertaining to a tweet such as Username, Screename, Location, Time of Tweet, the Tweet itself and lastly, the label for each tweet.
 classnames are->'Extremely negative' , 'Negative' , 'Positive' , 'Extremely Positive' , 'Neutral'.


# PREPROCESSING
After going through several steps of visualization of the dataset and how the data is distributed, the NLTK(famous library for NLP problems) is used for preprocessing.
Stopwords, symbols and other unnecessary stuff is deconsecrated from the Tweets and only pure tweets are left for model preparation.
Then, the dataset is then bifurcated into training and testing dataset. 
Using the sklearn library, the labels for the tweets are converted into one hot encodings to match the output of the model.

# MODEL
A BERT encoder and preprocessor is used to generate a high-performance model for the dataset.
The model is built using a functional API of the tensorflow framework to achieve an accuracy rate of 72% of the testing dataset.


Finally, a confusion matrix visualizes the performance of the model on both the training and testing dataset.
