Part 1: EDA - Loan_Data (R)
Part 2: Modellings - PredictInvestors (Python)


![alt tag](https://cloud.githubusercontent.com/assets/10266642/23363730/a731bea4-fd2e-11e6-9320-069cf747cd9d.png)

![alt tag](https://cloud.githubusercontent.com/assets/10266642/23363766/dfc1ea3c-fd2e-11e6-9055-4e6269dab76f.png)

Investment are categorized into 2 groups based on the ratio of average investment amount to the expected payment.

3 factors were used to measure the risk, and in all 3 of them, group B outdid group A:

Group A: Small average investment amount, higher risk, higher expected ROI.
Group B: Large average investment amount, lower risk, lower expected ROI.


Based on the information gained, I used Python to predict the number of investors who will invest in a particular loan.

I used a classification, to identify and seperate these trends, and then fit a regression to them individually. 
This approach is somewhat more complicated, but it works.

![alt tag](https://cloud.githubusercontent.com/assets/10266642/23798886/112a7514-05d9-11e7-9675-5623ff09e94a.JPG)

I saved 25% of the data for testing, and put all the training data available to search for the most suitable algorithms and parameters.

![alt tag](https://cloud.githubusercontent.com/assets/10266642/23798826/d84f9c24-05d8-11e7-9672-572b99540073.JPG)

The training data was then separated based on group and used to train regression models for the 2 different groups.

![alt tag](https://cloud.githubusercontent.com/assets/10266642/23798831/dbb64f48-05d8-11e7-803b-3d0a3a6e1279.JPG)

The test data was separated based on the group predictions.

![alt tag](https://cloud.githubusercontent.com/assets/10266642/23798827/d9d5fdfe-05d8-11e7-9f3a-294c6acaebac.JPG)

The test data was further separated, into true postive prediction, and false prediction (everything else). 
Then I put them in the model and evaluate the result.