## Detecting Hate Speech in Social Media
Here we try to implement the paper

Detecting Hate Speech in Social Media by Shervin Malmasi & Marcos Zampieri

https://arxiv.org/abs/1712.06427


Here is the abstract from the paper

    Abstract
    In this paper we examine methods to detect
    hate speech in social media, while
    distinguishing this from general profanity.
    We aim to establish lexical baselines for
    this task by applying supervised classification
    methods using a recently released
    dataset annotated for this purpose. As features,
    our system uses character n-grams,
    word n-grams and word skip-grams. We
    obtain results of 78% accuracy in identifying
    posts across three classes. Results
    demonstrate that the main challenge lies in
    discriminating profanity and hate speech
    from each other. A number of directions
    for future work are discussed

### Summary
- Data is preprocessed and transformed according to the methods stated in the paper
- Covered all the different vectorizers outlined in the paper and extracted many different set of features from the data
- Few utility methods were written to cover things like skipgrams
- Executed the classifier on all feature sets and listed the scores of all classifiers
- Implemented the baseline and oracle classifier
- Implemented a combined classifier that uses all features from all vectorizers
- Implemented the learning curve and found the effect of adding data on the classifier
- Plotted the confusion matrix
- Displayed sample tweets from each group of interest (Hate and Offensive) that are correctly and also incorrectly classified
- Implemented an ensemble classifier which is mentioned in the future work
- Tried NBSVM classifier from https://nlp.stanford.edu/pubs/sidaw12_simple_sentiment.pdf and achieved new state of art accuracy score of 78.634
