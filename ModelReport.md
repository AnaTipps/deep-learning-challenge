# Deep learning Charity Foundation Model Summary Report

## Overview

The purpose of Analysis: To predict the success of a foundation based on historic features of previous projects.

## Results

* Data Preprocessing: 

  - Target Variables: 'IS_SUCCESSFUL' feature, which is a binary value that indicates whether the money was used effectively or not
  
  - Features: All remaining columns other than the target column and the 'EIN' and 'NAME' columnms were used for model. 
  
  - Removed Columns: EIN and NAME colums, were removed since they are neither targets nor features.

* Compiling, Training, and Evaluating the Model

  - First Model Description:
  
    * Layers: 2
   
    * Nodes: 16, 8
    
    * epochs: 20
   
    * Activation Function: 'relu'
   
  - Optimized Model Description:
  
    * Layers: 4
   
    * Nodes: 80, 30, 16, 5
    
    * epochs: 50
   
    * Activation Function: 'swish'

  - Results Accuracy: 

    * First model: Accuracy: 72.7% Loss: 0.56
   
    * Optimized model: Accuracy: 73.1 % Loss: 0.56
    
    * Target accuracy was not achieved
 
  - Optimization steps: The second model uses two extra layers and more nodes in the original 2 layers, increases the epochs in addition to changing the activation function in an attempt to increase the accuracy.

### Summary

While the accuracy appears to improve for the second model it is not by a significant amount, the additional resources and processing time it requires are not justified.

A different model that can be used like the Random Forest Algorithm which could be a better alternative to Neural-Networks because it is more interpretable, robust to noise and outliers, and more scalable as it is relatively quicker to train.
