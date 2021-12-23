# Project 2 (EPFL Machine Learning Course CS-433)
# Sentence classification

This is a repository for all code of project 2

Members:

- Bohan Wang (321293)

- Ke Wang (326760)

- Siran Li (321825)

## Datasets 
1. News reports: 143, 000 articles from 15 American publications [[1]](#1).
2. Ted 2020 Parallel Sentences Corpus: around 4000 TED Talk transcripts from July 2020 [[2]](#2).
3. Wikipedia corpus: over 10 million topics [[3]](#3).
4. Topical-Chat: human dialog conversations spanning 8 broad topics [[4]](#4).

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

## References
<a id="1">[1]</a> 
A.   Thompson, (2017)
“All   the   news:   143,000   articles   from   15   americanpublications,”
https://www.kaggle.com/snapcrack/all-the-new

<a id="2">[2]</a> 
N.   Reimers   and   I.   Gurevych, (2020)
“Making   monolingual   sentence   em-beddings   multilingual   using   knowledge   distillation,” arXiv   preprintarXiv:2004.09813

<a id="3">[3]</a> 
W.   Foundation.   Wikimedia   downloads.
[Online].   Available:   https://dumps.wikimedia.org

<a id="4">[4]</a> 
K.  Gopalakrishnan,  B.  Hedayatnia,  Q.  Chen,  A.  Gottardi,  S.  Kwatra,A. Venkatesh, R. Gabriel, D. Hakkani-T ̈ur, and A. A. AI, (2019)
“Topical-chat:Towards  knowledge-grounded  open-domain  conversations.”  inINTER-SPEECH, pp. 1891–1895



