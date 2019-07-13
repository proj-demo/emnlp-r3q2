## Future Work
### Since word2vec embedding should contain semantics of the words already, synonyms should have similar embedding. How is the synonyms extension to relation indicators useful?  
<br />

##### In our work, Synonyms from Thesaurus.com are used to broaden the coverage of relation indicators in order to form a robust relational semantic space, which aims to capture the keywords of relations precisely.
##### The reason why we use external knowledge base instead of relying on pre-trained word vectors is that the synonyms obtained by Thesaurus.com is more reliable and accurate, whereas the pre-trained word vectors often produce unsatisfactory results regarding the cosine similarity of words. For example, the similarity between "good" and "bad" is 0.72, whereas the similarity between "good" and "amazing" is only 0.48.  Such errors and unexpected results will introduce more noise to our model. 
##### Although fine-tuning during training may adjust the word vectors to better suit for our task, more training data and model capacity are needed. This is exactly our motivation to incorporate external knowledge to deep neural network to reduce its reliance on training data while improving its performance. 
