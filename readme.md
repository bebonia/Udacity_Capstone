# Udacity DS Nanodagree Capstone Project - Customer Complaint Topic Modelling using LDA (Latent Direchlet Allocation)
---
# Introduction
---
Currently I am working as a business analyst in the banking industry in Australia. It is arguable that the number one priority for a consumer bank is to keep it's customers happy. As part of a running a business, complaints will naturally occur.

What could seperate a succesful business to a failing business is how each business handles complaints.

# Problem Statement
---
The aim of this project is to gain a greater understanding of a corpus of customer complaints by answering the question:

What are the hidden customer complaint topics?
LDA (Latent Direchlet Allocation) will be used to answer this and hopefully provide a proof of concept to be implemented in a real life scenario.

Once hidden topics have been found, analysis of the keywords of these topics can now be analysed and provide further insights for the business to improve and action.

# Objectives:
---
1. Preprocess customer complaint data, ready for ingestion of Machine Learning Models.
2. Create an LDA (Latent Direchlet Allocation) model to identify possible clusters of complaints into 'topics'
3. Analyse topics and obtain insights.

# Requirements and files
---

### Packages
The following packages are required to be installed in Python

1. Numpy
2. Pandas
3. Spacy
- Once Spacy is installed also run the following command in the terminal to complete the installation
- ``` python -m spacy download en_core_web_sm ```
4. Nltk
5. Sklearn
6. pyLDAvis
7. matplotlib
8. gensim
9. bokeh

### Files
The complaints dataset can be found in the complaints folder path:
``` \complaints\comcast_consumeraffairs_complaints.csv```

This file has been sourced from ```https://www.kaggle.com/archaeocharlie/comcastcomplaints```

| Column Name | Description                                              |
|-------------|----------------------------------------------------------|
| author      | Author of the complaint which includes name and location |
| posted_on   | Date the complaint was posted                            |
| rating      | Rating of the complaint from 0-5                         |
| text        | The complaint in text                                    |


# How to Run
---
Execute each code cell in the juypyter notebook.
Ensure Spacy has been installed properly (refer to Packages)

# Results
---
From the strategy we have identified the best model utilizing 6 topics with a coherence score of ~0.48.

From the visuals produced by pyLDAvis as well as looking the T-SNE Visualisation and SVD visualisation we can see theeperation between topics as well as see complaints who share similar themes.

Relative to our baseline model we have seen in improvement from a metric perspective (greater coherence score).




