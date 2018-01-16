## Detecting Hate Speech in Social Media
Here we try to implement the paper

Detecting Hate Speech in Social Media by Shervin Malmasi & Marcos Zampieri

https://arxiv.org/pdf/1712.06427.pdf


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
- We preprocessed the data and transformed it according to the methods stated in the paper
- We have covered all the different vectorizers outlined in the paper and extracted many different set of features from the data
- We wrote few utility methods to cover things like skipgrams
- We executed the classifier on all feature sets and listed the scores of all classifiers
- We implemented the baseline and oracle classifier
- We implemented a combined classifier that uses all features from all vectorizers
- We implemented the learning curve and found the effect of adding data on the classifier
- We plotted the confusion matrix
- We displayed some sample tweets from each of the groups of interest (Hate and Offensive) that are both correctly and incorrectly classified
- We implemented an ensemble classifier which is mentioned in the future work
- We tried NBSVM classifier from https://nlp.stanford.edu/pubs/sidaw12_simple_sentiment.pdf and achieved new state of art accuracy score of 78.634
