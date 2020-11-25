Sidenote: This was my first real life project.

## Project_PythonPredictions_Charity_Fundraise

This is a use case collaboration of Steven, Robin, Seppe and Kristof

### Goals

To predict which donors will donate again if a next campaing would take place.

### Table of contents

* [Technologies used](#technologies-used)
* [Approaches](#Approaches)
* [Results](#Results)
* [To Use](#To Use)

### Technologies used
- logistic regression
- clustering
- SVM
- Decision Trees
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

- Pandas insights
  Youngest person to start donating: 8
  Oldest person to start donating: 119
  12,9 % of donors do this spontaneously
  Average donation per gender is slightly higher for females:
    Male 	28.758326
    Female	29.551667
  Considering the whole lifetime of a donor:
  30120 is the highest total amount donated, 135 the mean and 50 the median

- Logistic regression
    Logistic Regression Accuracy:
	  0.991533689672662
    Balanced Logistic Regression Accuracy:
	  0.60645312317116
  --> potential improvements:
      Adding additional higher order features
          Different metrics 
          Precision
          Recall
          F1 Score
          Balanced classes

- 


### To use

aaaaaaaaaaaaaaaaaaaaaaaaa
```
file_name.py
```



