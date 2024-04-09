In this project, we will be analyzing the Twitter data we extracted using this api. This time, we extracted the tweets posted by the following six Twitter accounts: realDonaldTrump, mike_pence, GOP, HillaryClinton, timkaine, TheDemocrats.

For every tweet, we collected two pieces of information:

screen_name: the Twitter handle of the user tweeting and
text: the content of the tweet.
We divided the tweets into two parts - the train and test sets. The training set contains both the screen_name and text of each tweet; the test set only contains the text.

The overarching goal of the problem is to infer the political inclination (whether Republican or Democratic) of the author from the tweet text. The ground truth (i.e., true class labels) are determined from the screen_name of the tweet as follows:

R: realDonaldTrump, mike_pence, GOP
D: HillaryClinton, timkaine, TheDemocrats
We can treat this as a binary classification problem. We'll follow this common structure to tackling this problem:

preprocessing: clean up the raw tweet text using the various functions offered by the Natural Language Toolkit (nltk).
features: construct bag-of-words feature vectors.
classification: learn a binary classification model using scikit-learn.
Note that nltk supports optional corpora, toy grammars, trained models, etc. For this project, we have to manually install the stopwords list and WordNetLemmatizer. We'll begin by installing them:

Data sets available here:

tweets_train : [link](https://drive.google.com/file/d/1blOBpDKkB-h44lbBYdcdLoWw1toieEBQ/view?usp=sharing)

tweets_test: [link](https://drive.google.com/file/d/1z_T5bq-I-dYfd3mUlWdWCuZvGVjjMXb2/view?usp=sharing)

get_rare_words.output: [link](https://drive.google.com/file/d/11prpQFWCmdKDL27ZVu9THdCOA1TMPVPS/view?usp=sharing)
