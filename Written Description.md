# Project June
Andrew Seo

## Abstract:


## Design:


## Data:
I downloaded a Kaggle dataset of 130,000 rows scraped from WineEnthusiast in 2017. Almost all of the columns (except for price and vintage) are categorical variables, which required me to consolidate values in some columns (e.g. U.S., France, Other) and create dummy variables. 

## Algorithms:

**_Data Cleaning and EDA_**
1. Dropped unecessary columns and columns with too many missing values
2. Created vintage column from wine titles
3. Copied original dataset
4. Grouped remaining categorical features into a top 5 or top 10 with the rest being "other"
5. Mapped wines as "bad" or "good" depending on if they fell below the median or were greater than or equal to the median of all of the scores.

**_Model Picking_**
1. This could be considered Step 0 in a way but performed train_test_split twice to create 60-20-20 train-validate-test sets of the data.
2. KNN simple train/test split 
3. KNN cross validation including for loop looking for optimal K value
4. KNN retrain on optimal K value
5. Logistic Regression simple train/test split
6. Looked at precision-recall curve to determine different threshold and noted alternate probability on higher threshold
7. Logistic Regression cross validation including for loop looking for optimal C value but minimal impact so didn't retrain
8. Baseline Decision Tree model
9. GridSearchCV Decision Tree and retrain with results
10. Baseline Random Forest model
11. GridSearchCV Random Forest and retrain with results
12. Compare validation precision scores for all four models
13. Tested on logistic regression 

**_Model Findings (all figures validation precision scores)_**

KNN: 
- Baseline: 0.724
- Tuned: 0.770

Logistic Regression:
- Baseline: 0.752
- Tuned: 0.840

Decision Tree:
- Baseline: 0.720
- Tuned: 0.759

Random Forest:
- Baseline: 0.736
- Tuned: 0.748

## Tools
- Kaggle for dataset
- Pandas for EDA
- SKlearn for model selection, classification models, scoring metrics
- Matplotlib and Seaborn for visualization

## Communication

Presentation of findings attached to this written description. This includes visualizations and conclusions. 
