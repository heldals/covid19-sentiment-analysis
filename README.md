# Covid19 Sentiment Analysis
This is sentiment analysis (positive, neutral, negative) project about Indonesian government's actions in handling covid-19 on social media Twitter

# Method
1. Term Frequency — Inverse Document Frequency (TF-1DF)
2. Support Vector Machine
3. Kernel Radial Basis Function
4. Grid Search Parameter Tuning
5. K-Fold Cross Validation

# Project Steps 
1. Scraping 600 tweet data using hashtags or keyword #viruscoronaindonesia, 
#menkes, #indonesiaterserah, #PSBBJakarta, ‘psbbtotal’
2. Preprocess the dataset :
    - text cleaning
    - case folding
    - tokenizing
    - stopwords removal
3. Word weighting using TF-IDF
    - TF represents the number of occurrences of a
      term (t) in the document (d)
    - DF is the calculation of the number of documents in
      a term (t) that appears 
    - IDF to reduce the weight of a term if
      its appearance is widely scattered throughout the document
   The data from the TF-IDF weighting will be converted into vector for the SVM Training process
4. Split data into Training & Testing using K-Fold Cross Validation (K=10)
    - Data Training : 540
    - Data Testing : 60
5. Tuning hyparameter SVM (C & γ) to find the best parameter from training process
6. Training model using SVM to train the system classify
   sentiment with a best accuracy
7. The training result model will be used to classify the sentiments of 60
   tweet data test
8. Perform data visualization to present the classification of positive, negative, neutral sentiments

    
