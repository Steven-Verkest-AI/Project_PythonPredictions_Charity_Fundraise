Sidenote: This was my first real life project.

## Project_PythonPredictions_Charity_Fundraise

This is a use case collaboration of Steven, Robin, Seppe and Kristof

### Goals

To predict which donors will donate again if a next campaing would take place.

### Table of contents

* [Technologies used](#technologies-used)
* [Approaches](#Approaches)
* [Results](#Results)
* [Potential Improvements](#Potential Improvements)

### Technologies used
- logistic regression
- clustering
- SVM
- Decision Trees
- KNN
- could be used for further research -> Dimensionality Reduction & Principal Component Analysis

### Approaches
- First general preprocessing the data, removing outliers etc.
- Merge 2 fitting csv filtes together, so can be used easier later.
- Adding extra feature to the dataframe such as : Number of donations , Months as donor , Months since last gift, Frequency, Donates outside of campaign...
- Exploring data with pandas answer next questions:
  How frequently does a donor make donations?
  When was the last time a donor made a donation?
  What is the average donation amount of a donor?
  Is a donor making donation during reactivation campaign, or spontaneously
  Are there any regional differences?
 
### Results

- Pandas insights:
  Youngest person to start donating: 8
  Oldest person to start donating: 119
  12,9 % of donors do this spontaneously
  Average donation per gender is slightly higher for females:
    Male 	28.758326
    Female	29.551667
  Considering the whole lifetime of a donor:
  30120 is the highest total amount donated, 135 the mean and 50 the median

- Logistic regression:
    Logistic Regression Accuracy:
	  0.991533689672662
    Balanced Logistic Regression Accuracy:
	  0.60645312317116

- k-means clustering:
	no clear results, not a good algorithm for this type of problem
	
- regressions
	The model predicts that only 2 people will donate 30 euro or more.
	Donor 19048  --> [53.3319958]
	Donor 25804  --> [82.92821281]
	Conclusion -> It’s meaningless to send letters for the reactivation-campaign.

GENERAL CONLUSION
In general the results of the models are lacking. 
The accuracy is high but that is due to the highly imbalanced dataset we used to train with.
Other evaluation scores such as  Recall and F1 were really low, indicating that the models are not performing well.


### Potential Improvements

- logistic regression
	Adding additional higher order features
	Different metrics
	Precision
	Recall
	F1 Score
	Balanced classes

- regression
	Adding extra higher order features
	Using balanced data
	Feature engineering : L2 regularization with Ridge regression
	Feature engineering:  L1 regularization with Lasso regression
	Regression with Kernel Ridge with a polynomial kernel

- general potential improvements
	Trying to balance the dataset with using all the donors and selecting the same amount of random non-donors, then training the models, repeat this a few times, and 	   then take the average score of the training models.
	Upsampling those who donate, downsampling those who don’t




