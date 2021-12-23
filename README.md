# Project 2 (EPFL Machine Learning Course CS-433)
# Sentence classification

This is a repository for all code of project 2

Members:

- Bohan Wang (321293)

- Ke Wang (326760)

- Siran Li (321825)

## Datasets 
1. News reports: 143, 000 articles from 15 American publications
2. Ted 2020 Parallel Sentences Corpus: around 4000 TED Talk transcripts from July 2020
3. Wikipedia corpus: over 10 million topics
4. Topical-Chat: human dialog conversations spanning 8 broad topics

## Notes
The packages used in the project can be installed using:

``pip install transformers``

``pip install ntlk``

``pip install Sentencepiece``

## Structure
**train_models.ipynb:** contains the code to fine-tune transformers including BERT, GPT2, BIGBIRD, and BERT followed by downstream classifiers.

**random_forest.ipynb:** contains the code to ensemble five trained models with random forest.

**run.py:** contains the code to produce exactly the same .csv predictions which we used in our best submission to the competition system.

**proj1_helpers.py:** contains the functions provided by instructors

## Instuctions
The feature engineering and models evaluations can be reproduced in:

``project1.ipynb``

Note: we change the labels from {-1, 1} to {0, 1} for our logistic regression, which can make it model the probability.

You can reproduce the best prediction on the test set of the competition system:

``python run.py``


