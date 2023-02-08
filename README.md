# ensemble-learning
> The dataset has features of recording of vocal sounds of patients. These are being analysed in reference to presence or absence of a diagnosis of Parkinsons disease.
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
> Results
> - First the algorithms of Logistic Regression, KNN Classifier, Decision Tree classifier, Support Vector Classifier and Naive Bayes are implemented individually.
> - Thereafter they are stacked via StackModel with a final classifier of Logistic Regression and Support Vector Classifier.
> - Random Forests is then implemented as an ensemble technique.
> - Results are then compared.

| Model | Accuracy | Recall | Precision | F1 Score | AUC |
| :---: | :------: | :----: | :-------: | :------: | :-: |
| Logistic Regression | 85 | 97 | 83 | 90 | 77.7 |
| KNN | 86 | 97 | 85 | 91 | 80.3 |
| Naive Bayes | 75 | 68 | 93 | 78 | 78.49 |
| SVM | 80 | 100 | 77 | 87 | 68.4 |
| Stacking:SVM | 90 | 97 | 89 | 93 | 85.59 |
| Stacking:LG | 90 | 100 | 87 | 93 | 84.21 |
| Random Forest | 93 | 100 | 92 | 96 | 83.3 |
| Random Forest | 95 | 100 | 93 | 91 | 92.11 |

