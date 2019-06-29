# stackoverflow-word2vec Readme
This program demonstrates the use of gensim doc2vec word embeddings. 

<a href="https://colab.research.google.com/github/fmcooper/stackoverflow-doc2vec/blob/master/stackoverflow-doc2vec.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a>

******************************

1) Program use
2) Google Drive access

******************************

## 1) Program use

You will need to have a Google account to access colab. If you have never used colab before take a look <a href="https://colab.research.google.com/notebooks/welcome.ipynb">here</a>. After this, simply click on the following button to open this program in a new colab instance: 
<a href="https://colab.research.google.com/github/fmcooper/stackoverflow-doc2vec/blob/master/stackoverflow-doc2vec.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a>

The following variables are available to change: 
* ``NUM_TESTING`` should be a positive integer. If in testing mode then this program will run over the first ``NUM_TESTING`` samples of stackoverflow questions
* ``TESTING`` may be set as ``True`` or ``False``. Indicates whether we are in testing mode. 
* Result file locations may also be set. Please see Results section.

Note that data is not included in this repository due to size (~ 800Mb). The data is available from here: <a href="https://www.kaggle.com/stackoverflow/pythonquestions#Tags.csv">https://www.kaggle.com/stackoverflow/pythonquestions#Tags.csv</a> where the 'Questions.csv' file should be downloaded into a 'data' directory at the root of this repository.

## 2) Google Drive access

In order to save the model both during and after training, this program will ask you for google drive access. 

```
from google.colab import drive
drive.mount('/content/gdrive')
```

Please edit this line:

```
DATA_PATH = '/content/gdrive/My Drive/Colab/stackoverflow-doc2vec/data/Questions.csv'
```

To point at the data provided in this repository.
