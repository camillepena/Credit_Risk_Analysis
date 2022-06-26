# Credit_Risk_Analysis

## Overview of the analysis: 
	
In this analysis, we will be utilizing the different sampling methods to determine which is the best fit to determine loan risk in peer to peer lending services.

## Results: 

-Random Oversampling:  While the precision and recall scores are fairly highly for the low risk loans as expected the precision score for high-risk is only .01, and this method has one of our lowest accuracy scores of 64%.


![Naive Random Oversampling](https://user-images.githubusercontent.com/97993428/175815395-43143048-1b0e-49f6-8c8b-59a5be672379.png)


-SMOTE Oversampling:  While the precision and recall scores are fairly highly for the low risk loans like the Random Oversampling the precision score for high-risk is only .01, and this method has our lowest accuracy scores of 58%

![SMOTE Oversampling](https://user-images.githubusercontent.com/97993428/175815514-b177617d-6b7e-4b02-a66c-52db554eefe3.png)

-Undersampling:  The precision score for low-risk is 1.0 and the gap is starting to widen with the recall score on low-risk as well while the accuracy score is 99%.  The recall score for high-risk is high with undersampling, but the precision is .01.

![Undersampling](https://user-images.githubusercontent.com/97993428/175816102-658a467d-8597-466b-a1cf-fa34c7423c52.png)

-Combo:  Our Combo sampling scores are almost exactly the same as our undersampling values with a accuracy score of 99%.

![Combo](https://user-images.githubusercontent.com/97993428/175816267-2e554aa1-5e5f-4780-b949-ef8af884e05a.png)

-Balanced Tree:  The precision and recall scores with the low risk loans are 1.0 and .91 respectively putting this model at very close to perfect at accurately predicting low risk loans.  The precision score is .04 and a recall of .67 for the high risk loans.  

![Balanced Forest](https://user-images.githubusercontent.com/97993428/175816443-ea8433e9-3f2c-4694-a02d-443e6acfe977.png)


-Easy Ensemble:  The precision and recall scores with the low risk loans are 1.0 and 1.0 respectively putting this model at very close to perfect at accurately predicting low risk loans.  The precision score is .85, which is the highest we’ve had so far, and a recall of .38 for the high risk loans.  

![Easy Ensemble](https://user-images.githubusercontent.com/97993428/175816653-3dcbad5b-c0fa-4580-b126-aa0d84ff5678.png)


## Summary: 
For our analysis, the adaptative boosting was the best fit for our project.  Using the Easy Ensemble,  I was able to get the high risk loan precision and recall scores as close to 1 as possible while also closing the gap between them.  While my accuracy score was higher with a couple of my other techniques that was due to factors other than reliability given my other metrics didn’t align with an almost 100% accuracy score.
