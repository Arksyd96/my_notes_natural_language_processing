# Natural language processing

- Text preprocessing : process of cleaning the text data and make it ready to feed data to the model.
- Library to use : NLTK (Natural language toolkit).

### Text preprocessing techniques
- Expand contractions : expand contractions for better analysis and less tokens. Contractions dictionnaries can be found on the internet.  
  don't => do not.  
  aren't => are not.
- Lower casing : normalizing everything to lowercase makes less combinations to analysis (upper and lower case letters have a different code).  
  Hello and hello can be interpreted differently by a model.
  Lower case is preferred. Upper case can cause problems sometimes.
- Removing punctuation : less character for less combinations to analyse (Sometimes it can be useful to keep some punctiations for sentiment analysis).
  '!"#$%&'()*+,-./:;<=>?@\[\]^_`{|}~' or use string.punctuation.
- Removing digits and words containing digits.




