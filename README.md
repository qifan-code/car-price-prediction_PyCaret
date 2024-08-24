# car-price-prediction_PyCaret
This project is aiming for predicting car price based on given dataset by linear regression using PyCaret package

# 1. compare each model.
For PyCaret library, it compares different models and returns a table of model with its parameters. For this particular problem, it gives me the best one of using "Extra Trees Regressor" model which involves 0.0868 MSE on average. 

# 2. model tuning. 
Because I want to compare with linear regression and Extra Trees Regressor model, I tried to tune the parameters of those two models. 
Here is a comparision table: 
| Model | MSE before tune | MSE after tune | Final MSE(testing set) |
|-------|-----------------|----------------|------------------------|
|Extra Trees Regressor | 0.0868 | 0.1113 | 0.00|
|Linear Regression | 2125246465639139508224.0000 | 0.2366 |0.0752|

# 3. conclusion
PyCaret model is extremally useful when we want to supervised learning in traditional way. It compares with different types of model and provides hyper-parameter methods in a quick and efficient way. 
There are some problems remaining: 
a. MSE before tune, linear regression gives us an extremelly large value compared with the other method which makes me confused. 
b. Compared with MSE before and after tune, some model increase their MSE which doesnt make sense of hyper-parameter. 
c. Final MSE on testing set, Extra Trees Regressor gives 100% accuracy. This result seems unreliable. Maybe because of overfitting or testing set split etc. 
