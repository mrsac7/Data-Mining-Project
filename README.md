# Data-Mining-Project (CSE-362)
This repository contains source code for the Data Mining Project, IIT (BHU) Varanasi - Hate Speech Detection.

> **Guided By**: [Dr. Bhaskar Biswas](https://www.iitbhu.ac.in/dept/cse/people/bhaskarcse), Associate Professor, CSE, IIT (BHU) Varanasi.

### Group Members

- [Harshit Agrawal](https://github.com/harshitagrawal294) - 18074019 (CSE IDD Part 3)
- [Ashish Kumar](https://github.com/krashish8) - 18075068 (CSE B.Tech. Part 3)
- [Sachin Srivastava](https://github.com/mrsac7) - 18075070 (CSE B.Tech. Part 3)

### Hate Speech / Toxic Comment detection

- The project aims at improving the user experience of using any website for online chats, conversation and posts by flagging and removing the textual material containing hate and toxicity.
- Given any text or paragraph containing a few lines in natural language (such as English), the objective is to classify it as belonging to one of the following categories:- normal, obscene, threatening, insulting, toxic, severely toxic and hate.
- This is a multi-class classification problem as well as a multi-label classification problem, since a post can be abusive in multiple ways. The model will output the probability of the post belonging to each of the categories and based on a certain threshold (which can be tuned as a hyperparameter), a comment may be classified to be belonging to a category/set of categories

### Dataset

The dataset has been taken from [Conversation AI](https://conversationai.github.io/).

It consists of three files:
- Training Set ([train.csv](dataset/train.csv)): Contains comments with their labels (0 or 1).
- Test Set ([test.csv](dataset/test.csv)): We are required to predict the labels of these comments.
- Labels for test data ([test_labels.csv](dataset/test_labels.csv)): To evaluate our predictions on the test set.

### Embeddings

The download links of the pretrained embeddings used in the model:
- [Fasttext Embeddings](https://www.kaggle.com/vsmolyakov/fasttext/download)
- [GloVe Embeddings](https://www.kaggle.com/joshkyh/glove-twitter/download)
- [Word2Vec Embeddings](http://vectors.nlpl.eu/repository/20/2.zip)

### File Structure

- Project Description ([Project_Description.pdf](Project_Description.pdf))
- Presentation ([Presentation.pdf](Presentation.pdf))

The code is written in .ipynb files, which contain both the code and their outputs:
- Data Visualization ([Visualisation.ipynb](Visualisation.ipynb))
- SVM - Binary Relevance and Classifier Chains ([SupportVectorMachine.ipynb](SupportVectorMachine.ipynb))
- Logistic Regression - Binary Relevance and Classifier Chains ([LogisticRegression.ipynb](LogisticRegression.ipynb))
- Extra Trees ([ExtraTrees.ipynb](ExtraTrees.ipynb))
- XGBoost ([XGBoost.ipynb](XGBoost.ipynb))
- LSTM without pretrained embeddings ([LSTM_without.ipynb](LSTM_without.ipynb))
- LSTM with FastText embedding ([LSTM_fasttext.ipynb](LSTM_fasttext.ipynb))
- LSTM with Glove embedding ([LSTM_glove.ipynb](LSTM_glove.ipynb))
- LSTM with Word2Vec embedding ([LSTM_word2vec.ipynb](LSTM_word2vec.ipynb))

### Results

We have used AUC_ROC Score to evaluate the performance of the models. These are the results:

Model | Mean AUC_ROC Score
--- | ---
Support Vector Machines (Binary Relevance) | 0.66
Support Vector Machines (Classifier Chains) | 0.67
Logistic Regression (Binary Relevance) | 0.73
Logistic Regression (Classifier Chains) | 0.76
Extra Trees | 0.93
XGBoost | 0.96
**LSTM without pretrained embeddings** | **0.97**
LSTM with FastText embedding | 0.96
LSTM with Glove embedding | 0.88
LSTM with Word2Vec embedding | 0.85
