# TikTok-Video-Classification-Project
## Project Overview

TikTok, a leading platform for short-form mobile video, aims to foster inclusive, joyful, and authentic content creation. The data team focuses on increasing opinion videos, vital for platform growth. Observing that verified users are more likely to post opinions, the team aims to predict verified status based on video characteristics. This project involves developing a machine-learning model to classify videos as claims or opinions.
 We addressed skewed data, class imbalance & multicollinearity. The model achieved 74% precision.

<br> This project has 4 parts:
* Business Problem
* Data Understanding
* Modeling and Evaluation
* Conclusion


 
## Part 1: Business Problem
<img src="images/problem_10266358.png" width="100" height="100" align=left  >
The objective is to build a logistic regression model predicting whether a video is a claim or an opinion, using verified status as the outcome variable. This model will aid in prioritizing user reports efficiently and reducing backlog. Key questions include understanding the variables associated with user verification.




## Part 2: Data Undrestanding
<img src="images/survey_10266430.png" width="100" height="100" align=left  >
<br> 1. Descriptive analysis, hypothesis testing, and correlation matrices were used during exploratory data analysis.
<br> 2. Outliers were identified using interquartile range (IQR) and median due to strong skewness in certain variables.
<br> 3. Data preparation involved transforming categorical variables into numeric using one-hot encoding. 
<br> 4. Logistic regression assumptions were checked, including balanced classes and multicollinearity. 
<br> 5. To address class imbalance, upsampling was performed, and multicollinearity was resolved by removing one variable.




## Part 3: Modeling and Evaluation
<img src="images/creative-writing_10266412.png" width="100" height="100" align=left  >
* The model evaluation showed higher performance in predicting the "not verified" class.
* Precision: How many of the predicted positives were actually correct? (74% for "verified" class)
* Recall: How many of the actual positives did the model capture? (82% for "not verified" class)
* F1-score: Harmonic mean of precision and recall, a balanced measure. (71% for "not verified" class)





## Part 4: Conclusion
<img src="images/value_10266329.png" width="100" height="100" align=left  >

 The model seems to be performing better at predicting the "not verified" class. 

The precision and recall scores are taken from the "not verified" row of the output are more important. Because that is the target class that we are most interested in predicting. 


* Business recommendations based on the model include strategies to encourage more opinion videos, such as incentivizing verified status or providing tools for expressing personal viewpoints. 
* Further analysis could explore factors influencing user verification and tailor content recommendations accordingly.
