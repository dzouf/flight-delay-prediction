# Flight Delay Prediction

A machine learning project predicting flight delays using historical flight 
data built as a hands on exercise in classification , regression and model 
deployment.

## Overview

This project simulates flight data ( airline , origin , destination , time of 
day , weather conditions ) and trains two models :
- A **classifier** predicting whether a flight will be delayed ( yes or no )
- A **regressor** predicting how many minutes a delay will last

## Approach

1. **Data generation** : simulated 10,000 flights with realistic delay patterns 
   — weather ( rain , snow , fog ) , rush hour timing and airline-specific trends
2. **Feature engineering** : one hot encoding for categorical variables 
   ( airline , origin , destination , weather )
3. **Modeling** : Random Forest Classifier and Random Forest Regressor , 
   trained on an 80/20 train-test split
4. **Evaluation** : accuracy score for the classifier , RMSE for the regressor
5. **Feature importance** : identified which factors most influence delays
6. **Deployment** : built an interactive Gradio interface so users can input 
   flight details and get a live prediction

## Results

- Classification accuracy : **[fill in your number from the notebook]**
- Regression error (RMSE) : **[fill in your number] minutes**
- Top delay factors : distance , hour of departure and weather conditions 
  ( snow and rain ) ranked highest in feature importance

## Tech Stack

Python , Pandas , NumPy , Scikit-learn , Matplotlib , Seaborn and Gradio

## Interface

The final model is wrapped in a Gradio app where you can select an airline , 
route , time and weather condition to get a live delay prediction.

## Future Improvements

- Replace simulated data with a real dataset ( used US DOT flight delay data 
  on Kaggle ) to validate the approach on real world patterns ( can't use the real data i worked with for privacy matters)
- Try gradient boosting models ( XGBoost and LightGBM ) for comparison
- Add crossvalidation instead of a single train-test split
