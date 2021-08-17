# Natural language processing

- Text preprocessing : process of cleaning the text data and make it ready to feed data to the model.
- Library to use : NLTK (Natural language toolkit).

### Text preprocessing techniques
- Dealing missing values : check null values in the dataset.
- Removing URLs and HTML tags : in some NLP datasets (like tweets) we can find URLs and HTML tags. Those are not useful.
- Expand contractions : expand contractions for better analysis and less tokens. Contractions dictionnaries can be found on the internet.  
  don't => do not.  
  aren't => are not.
- Lower casing : normalizing everything to lowercase makes less combinations to analysis (upper and lower case letters have a different code).  
  Hello and hello can be interpreted differently by a model.
  Lower case is preferred. Upper case can cause problems sometimes.
- Removing punctuation : less character for less combinations to analyse (Sometimes it can be useful to keep some punctiations for sentiment analysis).  
  '!"#$%&'()*+,-./:;<=>?@\[\]^_`{|}~' or use string.punctuation.
- Removing digits and words containing digits : makes the text cleaner. Sometimes it's also important to keep words containing digits (for example twitter usernames).
- Removing stop-words (**Important**) : stopwords do not provide any valuable information and thus, we can delete them.  
  ``from nltk.corpus import stopwords``
- Stemming and Lemmatization :
  * Stemming : 
  * Lemmatization :
- Removing extra spaces :D.
- Tokenization (**Important**) : spliting texts into array of words. Punctuation can be considered as tokens in some cases.  
  We can use NLTK tokenizer : ``from nltk.tokenize import word_tokenizer``.




