# Credit Risk Analysis Model Performance

For this project we used a selection of 6 differrent types of machine learning models to analyze and predict credit risk for perspective loan applicants. We compared balanced accuracy scores, F1 scores, and more to determine which model was the most accurate and should be used. This is a summary of our findings.

# Scores

Here is a list of the all the total scores for each model, beginning with the precision, recalled, F1, and other scores in order of the models we tested. Following that is the balanced accruacy scores in descending order.  


Oversampling Scores  
<img src="https://github.com/coryknuth/credit_risk_analysis/blob/a2cd54440175f2e902851eafc062dc44b5b22f3a/screenshots/oversampling%20scores.png" width="800"/>

SMOTE Oversampling Scores  
<img src="https://github.com/coryknuth/credit_risk_analysis/blob/a2cd54440175f2e902851eafc062dc44b5b22f3a/screenshots/smote%20oversampling%20score.png" width="800"/>

Undersampling Scores  
<img src="https://github.com/coryknuth/credit_risk_analysis/blob/a2cd54440175f2e902851eafc062dc44b5b22f3a/screenshots/undersampling%20scores.png" width="800"/>

Combination Scores  
<img src="https://github.com/coryknuth/credit_risk_analysis/blob/a2cd54440175f2e902851eafc062dc44b5b22f3a/screenshots/combination%20scores.png" width="800"/>

Random Forest Scores  
<img src="https://github.com/coryknuth/credit_risk_analysis/blob/a2cd54440175f2e902851eafc062dc44b5b22f3a/screenshots/random%20forest%20scores.png" width="800"/>

Adaboost Scores  
<img src="https://github.com/coryknuth/credit_risk_analysis/blob/a2cd54440175f2e902851eafc062dc44b5b22f3a/screenshots/adaboost%20scores.png" width="800"/>


## Balanced Accuracy Scores

Adaboost:             0.931  
Random Forest:        0.683  
SMOTE Oversampled:    0.662  
Oversampled:          0.648  
Combination Sampling: 0.640  
Undersampled:         0.600  


# Summary

We dertermined from the above that the two ensemble learning algorithms we tested may be the best choices. The Adaboost method returned the highest balanced accuracy score, although the precision for predicting high risk loans was extremly low at 9%. It's possible this overall accruacy score was inflated by overpredicting loans as low risk, and having a disproportionate count of the input data being low risk. Further testing is required to confirm the performance of this method.  

The Random Forest method scored second highest on balanced accuracy at .683 overall. The kicker is, the prediction precision for high risk loans was much higher than with the Adaboost method. The precision metric was .88 on predicting high risk loans, though the F1 score was a bit low at .52. The precision performance is encouraging, it will require further testing to confirm that performance.  

None of the other models demonstrated near the performance combination of accuracy and precision represented by the random forest algorithm. Though, given the results we have shown, it's possible our data was corrupted or incorrectly imported. We recommend further testing by re-analyzing all of the algorithms using another dataset to compare results against these to confirm if Random Forest is the best choice.  


