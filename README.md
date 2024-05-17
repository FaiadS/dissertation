# dissertation
This is the code from my dissertation. The actual document will be made public after it is marked. What I roughly did
was use data from openpowerlifting.org to create 3 ML models to predict an athletes maximal lift on squat, bench press
and deadlift. The functionality for using this yourself was not completed though the models were trained and achieved good
accuracy on the data (equal to latest work done on this except squat which performed slightly better than the cutting edge).
Evolutionary algorithms were played around with though this is more to do with the report/ investigation rather than the code.

The ipynb file must be opened in Google Colab (the simplest way I found to do this was to upload it to a google drive and open it from there).
The steps are labelled after the top comment of each cell. Some steps include options depending on which discipline you want to predict.
Before the final steps you can tune hyperparams using either grid/random search or a genetic algorithm (takes a while).
If you tune hyperparameters you MUST then change them in the Regression Models Code or they will not be applied.

Steps to run:

1. EA Setup
2. Setup
3. (NOT IN NOTEBOOK) Download data from https://openpowerlifting.gitlab.io/opl-csv/bulk-csv.html
3. Download Data (Ensure file path is correct)
4. Data Processing Functions
5. Preprocess
6. S seperate squat data OR B seperate bench data OR D seperate deadlift data
7. S train, val, test OR B train, val, test OR D train, val, test (ensure you choose the same lift as last step)
(Hyperparameter Tuning with grid and random search - tune hyperparams)
(RandomForest Genetic Algorithm - tune hyperparameters with a genetic algorithm)
8. Regression Models
