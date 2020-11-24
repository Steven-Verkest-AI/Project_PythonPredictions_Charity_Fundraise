Author: Steven Verkest
Team: Seppe Seghers, Wim Christaansen, Steven verkest

--------------------------------------------------

GOALS

Predict if a person is going to fund or not. (start project = 7/9)
Present work on 17/9 , explain models and conclusion, show list with predictions


1. Calculate the target for train and test data: All candidates donors from the campaign selections
who actually made a donation (information found in the gifts table)
2. Construct features. You can use information available in the donors table, but also information in
the gift table. For the latter, mind the timeline! Only information known before the event should be
used to train a model to make prediction.
3. Use a feature selection algorithm to select relevant variables (Optional).
4. Construct a model. You can use any type of algorithm. Compare the performance of different
models and check whether the models are interpretable.
5. Evaluate the model using AUC, but also lift and cumulative gain curves.
6. Try to make a business case using the campaign information. How much your model would have
increased the performance of the campaigns?




---------------------------------------------

TASKS

cleaning data ->
- explore data
- clean data
- find extra features

train models --> Logistische regressie / SVM  / Decision Trees /  Dimensionality Reduction   /  Clustering  

- evaluate models with test set
- evaluate models with extra test set (on 14/9)

deployment ->
- Save the models as an .h5
- Make a webpage with Flask
- load models into Flask 
- safe Flask into docker container 
- Deploy the container on Heroku 

● How frequently a candidate donor makes donations?
● When was the last time a candidate donors made a donation?
● What is the average donation amount of a candidate donors?
● Is a candidate donors making donation during reactivation campaign, or spontaneously?
● You can look at this variable over the short term (last months), long term (last years) and/or
lifetime

---------------------------------------------------

WEBAPP

You can try the webapp on -> heroku.com ... -> todo

------------------------------------------------------

TECHNICAL

- Logistic Regression Model
- SVM Model
- Decision Trees Model
- Dimensionality Reduction
- Clustering

---------------------------------------------------------

CONTENTS

all files of the project explained with their content
