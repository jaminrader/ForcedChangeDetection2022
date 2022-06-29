README.txt, for Detection of Forced Change with Combined Fields using Explainable Neural Networks (Journal of Advances in Modeling Earth Systems)
DOI: https://doi.org/10.1029/2021MS002941
Jamin Rader, Dept. of Atmospheric Science, Colorado State University; 2022

#####################################################
List of Notebooks:

**** TOE_classification.ipynb ****

Standardizes the input data. Trains a neural network to predict the year using 
fuzzy classification. Calculates performance statistics (loss, Pearson's r, RMSE) 
for the models. 

Plots the loss curve, and prediction versus truth plots (Figure 3, Figure 8, Figures
S10-12)


**** TOE_classification.ipynb ****

Same as TOE_classification.ipynb, but for training 100 different models with various 
train/test splits.


**** LRP.ipynb ****

Performs LRP on trained neural networks. Computes k-means clustering across LRP maps.


**** playground.ipynb ****

Majority of the plots, assumption checking, and data exploration.


**** TOE_classification_architecture_tune.ipynb ****

Testing various neural network architectures (Figure S2)


#####################################################
Plots and Models:

Find pre-trained models and their specs (in a pickle file) under models/
Corresponding learning curves and performance plots can be found under plots/


#####################################################
List of Pre-trained Models:

model1.h5: Trained on annual-mean temperature
model2.h5: Trained on annual-mean precipitation
model3.h5: Trained on annual-mean T and P combined
model4.h5: Trained on seasonal-mean T
model5.h5: Trained on seasonal-mean P 
model6.h5: Trained on seasonal-mean T and P combined
model7.h5: Trained on monthly-mean T
model8.h5: Trained on monthly-mean P 
model9.h5: Trained on monthly-mean T and P combined
model10.h5: Trained on seasonal-mean extreme precip over the Americas


#####################################################
Sample Data

A sample of standardized annual-mean temperature data over the land grid points of
the Americas from 1980-2098. This can be run through TOE_classification.ipynb to 
see how the neural network predicts the year.
