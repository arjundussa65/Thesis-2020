# Thesis-2020
This repository contains the implementation of Data Collection from Twitter, processing and finetuning of BERT and XLNet models for multiclass classification problem
## How to use?
### Extracting and preparing data
Create an account in Colab.

run extraction.ipynb to download tweets from Twitter. Using this code, historical tweets also can be extracted.

run dataset_creation.ipynb notebook to filter the data using additional hashtag filters. In my case, I was using industry specific hashtags as per my need.

Then execute Data_preprocessing.ipynb to do some preprocessing tasks. Additional steps can be added as per the task.

Polarity assignment.ipynb is used to label the dataset with Textblob and Vader scores.

After that Data_Exploration is to understand the data prepared.

## Modelling
This implementation is to understand Dropout and Mixout regularization techniques while finetuning BERT and XLNET. Mixout is implemented only on the classifier layer.

BERT.ipynb, XLNet model.ipynb are for dropout and mixout implementations without any sampling. 

BERT with undersampling.ipynb and XLNet with undersampling.ipynb are after sampling to prove that this technique works better when there less training examples.

Mix.py and mixout.py are taken from https://github.com/bloodwass/mixout a paper published https://arxiv.org/abs/1909.11299


