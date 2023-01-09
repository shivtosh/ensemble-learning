# ensemble-learning

Attribute Information:
* name - ASCII subject name and recording number
* MDVP:Fo(Hz) - Average vocal fundamental frequency
* MDVP:Fhi(Hz) - Maximum vocal fundamental frequency
* MDVP:Flo(Hz) - Minimum vocal fundamental frequency 
* MDVP:Jitter(%),
* MDVP:Jitter(Abs),
* MDVP:RAP,
* MDVP:PPQ,
* Jitter:DDP - Several measures of variation in fundamental frequency 
* MDVP:Shimmer,
* MDVP:Shimmer(dB),
* Shimmer:APQ3,
* Shimmer:APQ5,
* MDVP:APQ,
* Shimmer:DDA - Several measures of variation in amplitude
* NHR,HNR - Two measures of ratio of noise to tonal components in the voice status - Health status of the subject (one) - Parkinson's, (zero) - healthy RPDE,D2 - Two nonlinear dynamical complexity measures
* DFA - Signal fractal scaling exponent
* spread1,spread2,PPE - Three nonlinear measures of fundamental frequency variation 
* car name: string (unique for each instance)


1. Load the dataset
2. It is always a good practice to eye-ball raw data to get a feel of the data in
terms of number of records, structure of the file, number of attributes, Mention a few comments in this regard.
3. Using univariate & bivariate analysis to check the individual attributes for
their basic statistics such as central values, spread, tails, relationships
between variables etc. mention your observations 
4. Splitthedatasetintotrainingandtestsetintheratioof70:30
(Training:Test) 
5. Prepare the data for training - Scale the data if necessary, get rid of missing
values (if any) etc 
6. Trainatleast3standardclassificationalgorithms-LogisticRegression,
Naive Bayes’, SVM, k-NN etc, and note down their accuracies on the test
data 
7. Train a meta-classifier and note the accuracy on test data 
8. TrainatleastonestandardEnsemblemodel-Randomforest,Bagging,
Boosting etc, and note the accuracy 
9. Compare all the models (minimum 5) and pick the best one among them
