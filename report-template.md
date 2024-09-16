# Report: Predict Bike Sharing Demand with AutoGluon Solution
KANWAR PREET KAUR

## Initial Training
### What did you realize when you tried to submit your predictions? What changes were needed to the output of the predictor to submit your results?
The predictions in the first model was suppose to have some negative value but since there was none no changes were needed. 

### What was the top ranked model that performed?
WeightedEnsemble_L3 with -53.156712 score_value.

## Exploratory data analysis and feature creation
### What did the exploratory analysis find and how did you add additional features?
So we discovered that the datetime graph was not as useful so we created hour, day and year features in order to understand better that when in the hour of the day are bike sharing are most useful and so on.

### How much better did your model preform after adding additional features and why do you think that is?
The score defined improved from -53.156712 to  -50.218716. The added features model became better because we focused on the relevant things of the model. Like changing the datetime to more important factor hour. Changing the integer type to category for season and weather.

## Hyper parameter tuning
### How much better did your model preform after trying different hyper parameters?
The hyper parameters in this model was not that effective and hence it was not needed. 

### If you were given more time with this dataset, where do you think you would spend more time?
If I was given more time I would try to further analyse the dataset and work on adding more additional features in order to improve the models.

### Create a table with the models you ran, the hyperparameters modified, and the kaggle score.
model	hpo1	hpo2	hpo3	score
0	initial	presets="best_quality"	Automatic settings	Automatic settings	1.80060
1	add_features	presets="best_quality"	Automatic settings	Automatic settings	0.54498
2	hpo	presets="best_quality"	GBM/RF/XT/XGB models	search_trategy: bayesopt	0.53682

### Create a line plot showing the top model score for the three (or more) training runs during the project.
![Alt text](image-3.png)

### Create a line plot showing the top kaggle score for the three (or more) prediction submissions during the project.
![Alt text](image-4.png)

## Summary
I think that this project was a success we worked more on autogluon which is one of the most complex framework and has various models trained to find the best one for the dataset. We covered all the following things :
1)Autogluon framework : Processed , created and tuned the ML models 
2)EDA:Exploratory Data Analysis was done using Pandas such as creating line graphs and histograms for analysis 
3)Hypertuning: We hypertuned our model and learned about how to use various settings. Although it didn't improve our model but it was a good practice.  
