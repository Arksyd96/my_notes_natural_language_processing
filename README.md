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
- Removing extra spaces :D.
- Tokenization (**Important**) : spliting texts into array of words. Punctuation can be considered as tokens in some cases.  
  We can use NLTK tokenizer : ``from nltk.tokenize import word_tokenizer``
- Removing stop-words (**Important**) : stopwords do not provide any valuable information and thus, we can delete them.  
  ``from nltk.corpus import stopwords``
- Stemming and Lemmatization :
  * Stemming :Stemming usually refers to a crude process that chops off the ends of words in the hope of achieving this goal correctly most of the time, and often includes the removal of derivational units (the obtained element is known as the stem).  
    ``i saw an amazing thing`` => ``i s an amazing thing``
  * Lemmatization : lemmatization consists in doing things properly with the use of a vocabulary and morphological analysis of words, to return the base or dictionary form of a word, which is known as the lemma.  
    ``i saw an amazing thing`` => ``i see an amazing thing``
- Remove tokens with length <= 2 :D.
- Vectorization (**Important**) : the process that follows the tokenization and deletion of stop-words is the vectorization. Vectorization is the transformation of the data from text into numbers (floats). There are many techniques and ways of vectorizing tokens :
  * Count vectorizer : transforms tokens into an array of theur occurences in a given sequence.  
    ``This document is the second document. + ['and', 'document', 'first', 'is', 'one', 'second', 'the', 'third', 'this'] => [0 2 0 1 0 1 1 0 1]``
  * N-grams : n-grams method combines sequences of n words to create new tokens. Each combination will be represented with the rest of the tokens as indexes.  
    ``if n=2, i.e bigram, then the columns would be — [“I love”, “love this”, ‘this article”]
      if n=3, i.e trigram, then the columns would be — [“I love this”, ”love this article”]``




