# IBM Acquisition Team Recommendations
In this project I have put myself in the position of a data scientist for IBM making a presentation to the acquisition. I look at current workers and their 
output and make a predictive model for the best workers. In order to this, I engineer a variable, called 'Quality' to predict. Additionally, I also predict 
'attrition,' which means a worker will quit within the next 2 years. In this manner, I am completing a 2-variable prediction for a holistic hiring approach.
The dataset used is located in the repository as [attrition.csv](https://github.com/micdwill/IBM-Hiring/blob/master/attrition.csv).

## Data Cleaning
It is important to note that when predicting both quality and attrition, all variables that can only be calculated following the hire of a worker were removed. 
This ensures that my model can be used when viewing a prospective hire. As a byproduct of this, quality is not used when predicting attrition and vice 
versa. Additionally, variables with too much predictive power were removed.

## Methods
A stacked decision tree model was utilized. Within this stacked model, I use GLM, KNN, SVM, Neural Networks, and an initial Decision Tree. This is done for 
both variables I am predicting. I leveraged a cost matrix for both decision trees with the intention of avoiding false negatives. Following this, 
I choose to hires workers who are both predicted to be quality and stay with IBM long-term. Results are displayed.

## Results
Results can be seen in [IbmHiring.pdf](https://github.com/micdwill/IBM-Hiring/blob/master/IbmHiring.pdf). My model was sucessful, as it leads to an additional 
income of about 75 extra dollars per hire (based on my initial assumptions). The commented code in RMarkdown format that leads to this conclusion can be seen in
[IbmHiring.Rmd](https://github.com/micdwill/IBM-Hiring/blob/master/IbmHiring.Rmd).
