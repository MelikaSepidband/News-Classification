# News-Classification
Persian news classification with Naive Bayes Classifier  
The data is in this link : https://drive.google.com/file/d/1JY7LGYiB5xLAB2QQZmmjZhL3gd76AVE2/view  
The data is persian news with their categories.  
The goal of this project is to build a Naive Bayes classifier for news classification.  

class DataPreprocessor :  

read_data : Concatening "title" and "text" of the news to a new column = "input"  

plot_distribution : shows the distribution of categories in news data in a diagram.  

clean_text : deleting characters that are not main characters, replace numbers with "N".  

count_words : returns a dictinary of tokens and their frequencies.  

map_word_index : returns dictinaries WordToIndex, which maps each token to a number, and IndexToWord, which maps each number to a token.  

tokenize : gets a string and returns the number of each token in the string.  

frequent.txt : 200 most frequent tokens in the data.  

WordToIndex.txt : tokens and their corresponding number.  

class NaiveBayesClassifier :  

count_word_per_class : returns the number of each token in each category.  

calculate_word_log_prob_per_class : gets a word and calculates probability of being in each category.  

calculate_log_prior : calculates log likelihood of each category.  

predict : gets a string and calculates the probability of being in each category and returns the most probable category.  

evaluate : gets a data and returns Accuracy, Precision, Recall and F1_score of the prediction.
