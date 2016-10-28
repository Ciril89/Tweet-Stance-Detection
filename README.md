Prerequisites

1)	Python 2.7.8
2)	Python Libraries:
  a)	NumPy
  b)	Pandas
  c)	sci-kitlearn (sklearn)
  d)	Natural Language Toolkit (nltk)
  e)	Natural Language Toolkit Data (words, punkt)
To download this data, the following commands need to be executed from a the python shell:

import nltk
nltk.download('punkt')
nltk.download('words')
3)	GloVe prebuilt model, which can be downloaded from http://nlp.stanford.edu/data/glove.twitter.27B.zip
4)	Input data and programs that are provided with the submission.

Steps of Execution

1)	The input files training.txt, test-gold.txt, the python programs and the gloVe file glove.twitter.27B.200d.txt should be in the same folder or file name changes must be made in the programs accordingly.
2)	The default classifier is SVC with linear kernel. To change this, one or more of lines 30, 68, 72, 81 and 83 of tweetStancePredictor.py have to be changed as desired.
3)	The program tweetStancePredictor.py  is the main program and it is the only one that has to be invoked explicitly. Vectorize.py  is a module that is invoked implicitly.
4)	Once the program tweetStancePredictor.py  is executed, the user is asked to input choices for vectorization(either glove or TFIDF) and evaluation(either k-fold or with test data).
5)	The results will be written to log file in the same folder as the programs. The logfile will be named logSVC.txt or logRFC.txt or logGBC.txt depending on what classifier was used. The results will be printed on the console as well.
