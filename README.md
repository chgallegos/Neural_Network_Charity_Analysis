# Neural_Network_Charity_Analysis

## Overview

The overall goal of this project is to use a provided dataset to create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.

----
## Results

In order to perform the study, the analysis will be divided into 3 parts 

#### 1) Preprocessing Data for a Neural Network Model
#### 2) Compile, Train, and Evaluate the Model
#### 3) Optimize the Model

### Data Preprocessing

The target variable for the model was determined to be the variable IS_SUCCESSFUL. The rest of the variables will be considered features.

![Screenshot](https://github.com/chgallegos/Neural_Network_Charity_Analysis/blob/main/Resources/target.png)

It was also considered to drop the following columns that were not beneficial for the model

![Screenshot](https://github.com/chgallegos/Neural_Network_Charity_Analysis/blob/main/Resources/dropped_columns.png)


### Compiling, Training, and Evaluating the Model

I decided to use 2 layers with 25 and 15 nodes. for both layers, the use of the "relu" activation was chosen and for the output layer, the "sigmoid" activation was selected.

![Screenshot](https://github.com/chgallegos/Neural_Network_Charity_Analysis/blob/main/Resources/model.png)

This model provided an accuracy of 72.59 %

![Screenshot](https://github.com/chgallegos/Neural_Network_Charity_Analysis/blob/main/Resources/model_accuracy.png)

### Optimize the Model

The optimization process was done three times, while the layers and activations were changed while maintaining the 100 epochs. 

Unfortunately, the target model performance was not achieved, yet an understanding of how the different activation methods as well as amount of layers/nodes can influence the accuracy. The takeway is that on the third optimization attempt, a third layer was added which produced a small increase in accuracy.

#### Optimization 1
![Screenshot](https://github.com/chgallegos/Neural_Network_Charity_Analysis/blob/main/Resources/optimize1.png)
![Screenshot](https://github.com/chgallegos/Neural_Network_Charity_Analysis/blob/main/Resources/target1.png)

#### Optimization 2
![Screenshot](https://github.com/chgallegos/Neural_Network_Charity_Analysis/blob/main/Resources/optimize2.png)
![Screenshot](https://github.com/chgallegos/Neural_Network_Charity_Analysis/blob/main/Resources/target2.png)

#### Optimization 3
![Screenshot](https://github.com/chgallegos/Neural_Network_Charity_Analysis/blob/main/Resources/optimize3.png)
![Screenshot](https://github.com/chgallegos/Neural_Network_Charity_Analysis/blob/main/Resources/target3.png)

## Summary 

I believe that my model did not increase substantially to the target accuracy because I did not drop unnecessary column information. I do believe that I used the appropriate activation method as the numbers were consistent when they were going through the epochs. I would also consider other methods of machine learning to see how they would perform, in the case of the data that we have available for this dataset, I would consider revising the columns and after transforming them into tabular, to use a random forest classifier. 
