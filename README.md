# Web-Science
Recommending Systems

This project consists of 3 main ipynb files:
* main.ipynb:
    It has the majority of the code with 3 classes.
    * SentAnalyzer
        - init: Reads in and stores the SST data
        - checkBalance: label counting
        - nGrams: calculates nGrams
        - lengthCorrelation: checks the length correlations
        - textTfidfValues: returns the tf-idf values in descending order
    (Amazon Review - only reads in but do nothing particular)
    * CrowdSourcer
        Collaboration evaluation.
        - init: Reads in the GlobalSheet
        - calcKrippendorff: Calculates the Krippendorff coef
        - trainByCS: Trains from the data the VoteClassifier
        - checkPrediction: Runs the predictions
    * Recommender
        Inharited from the SentAnalyzer. 
        - init: read in
        - getDocTermMtx: creates Document-Term Matrix
        - dimensionReduce: Reduces the size of the word vector matrix
        - predictWithModels: ---- (place of tryings)
    (The comperision of the trainings)

* collabEvalOwn.ipynb
    This contains my own solution for the collaboration.
    (Well commented)

* sstManual.ipynb
    This contains my own solution for the collaboration
    * Analyzer
        - init: Reads in and stores the SST data
        - processData: Sorts by labels and counts nGrams
        - sortData: Sorts the counted nGrams
        - (checkCounting: Checks the counts in of the labels)
        - lengthAnalysis: Word length check
        - lengthCorrelation: length corralation
        - printFrequent: word frequence
        (goes throw all the 3 sets - train,dev,test)
