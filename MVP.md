# Project Pinot

## New Abstract:
I have shifted away from my original basketball idea to a wine review dataset. With this data, I hope to look at the features that contribute most to a "good" score (with review scores below the median labeled as "bad" and equal to greater than the media as "good"). 

## Data:
I downloaded a Kaggle dataset of 130,000 rows scraped from WineEnthusiast in 2017. Almost all of the columns (except for price and vintage) are categorical variables, which required me to consolidate values in some columns (e.g. U.S., France, Other) and create dummy variables. One dummy variable I have kept in so far is the reviewer. It may be interesting to see if certain reviewers tend to give higher scores and if a maker should try to somehow attempt to get their wine reviewed by one taster over another. 

## Initial Results and Visuals:
I have started to go through the modeling process, starting with KNN and Logistic Regression. Initially, my instinct was to pick accuracy as the metric of choice because the classes were relatively balanced but I'll look at the other scoring metrics as well. 

![Screen Shot 2021-10-26 at 2 13 36 AM](https://user-images.githubusercontent.com/89528655/138819206-d34ab290-3f78-4139-93d9-96778bbe9b4f.png)

We have a plot of accuracy vs different values of K. While the accuracy does incrementally increase with K and I trained on K = 30 as a result, I wonder if I should pick a smaller value of K to train on as 30 feels like too much smoothing. The initial results of a k=30 model is a best score of 0.735 accuracy.

![Screen Shot 2021-10-26 at 2 56 01 AM](https://user-images.githubusercontent.com/89528655/138824385-137e83ed-b488-4f71-9ec6-8f67982e234f.png)

We have a logistic regression confusion matrix. The precision and recall scores asssociated with this plot are 0.7586 and 0.7347 respectively. Accuracy was 0.727, so a smidge lower than KNN. 

## Next Steps/Concerns:
- Decision trees, random forests, bootstrapping, ensembling   
- Is initial 0.735 accuracy considered too high? How do I inspect for data bleed?
- Feature engineering to try to increase scores. 
- Make a decision on reviewer columns. Should I only use columns that are objective?
- Is accuracy the best metric to look at? It feels like the lectures discouraged this.
- What exactly is my stopping point? Having trouble delineating between Results and Conclusions.  
