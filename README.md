# Vector Space Proximity Workshop

## Group Info:
- Group: Group1
- Team Members:
    - Ce Chen | 9007166
    - Zhuoran Zhang | 9048508

## GitHub Link
https://github.com/chence/VectorSpaceProximityWorkshop.git

## Dependencies
```shell
$ pip install numpy pandas scikit-learn nltk
```

## Main Notebook
- `VectorSpaceProximityWorkshop.ipynb`

## Overview
This project implements a basic information retrieval (IR) system using vector space models. The system processes a text corpus, converts documents into vector representations, and retrieves relevant documents based on cosine similarity.

## Dataset
We used the **20 Newsgroups dataset**, which contains a collection of approximately 11,000 text documents across multiple topics such as technology, politics, sports, and science.

Source:
https://scikit-learn.org/stable/datasets/real_world.html#newsgroups-dataset

## Preprocessing
The preprocessing pipeline includes:
- Lowercasing
- Removing punctuation and non-alphabetic characters
- Tokenization
- Stopword removal
- Stemming (Porter Stemmer)

## Vector Representations
We implemented and compared the following representations:
- Binary Incidence Matrix
- Term Frequency (TF)
- Log-scaled TF
- TF-IDF

## Retrieval Method
Documents are ranked using **cosine similarity** between query vectors and document vectors.

## Queries
We defined at least five information needs and corresponding queries to test the retrieval system.

## Evaluation
For selected queries, we manually created relevance judgments and computed:
- Precision
- Recall
- F1-score
- Precision@K
- Average Precision (AP)
- Mean Reciprocal Rank (MRR)

## Results
TF-IDF representation generally provided better ranking quality compared to binary representation, especially for queries involving common terms.
