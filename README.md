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
