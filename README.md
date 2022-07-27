# Neural Network Charity Analysis

## Purpose

The non-profit organization AlphabetSoup has requested a robust analysis using neural networks to predict where the organization's donation dollars can be most effective. Using a neural network to evaluate internal data on organizations that have received funding, AlphabetSoup should be able to better predict risky investments and funnel their dollars to successful endeavors. 

## Results

### Data Preprocessing

1. The variable "IS_SUCCESSFUL" was the primary target of this analysis. This variable identified whether or not the organization was successul
2. All variables other than removed and "IS_SUCCESSFUL" were considered in this analysis. 
3. The variables "EIN" and "NAME" were both removed from this dataset because they were inconsequential to the analysis.

### Compiling,Training, and Evaluating the Model

![alt text](https://github.com/sever1sd/Neural_Network_Charity_Analysis/blob/d776f57e7b342ab873665fadd46ec3e0c54ddc21/Resources/Neural%20Network.png)

1. The initial model had 2 hidden layers with 80 and 30 neurons each. The activation methods used were "relu" and "sigmoid."
2. This version of the model did not achieve target performance. After 100 epochs, the peak accuracy was 0.5438 with a loss of 1.1444. This is well below the 75% threshold.
![alt text](https://github.com/sever1sd/Neural_Network_Charity_Analysis/blob/d776f57e7b342ab873665fadd46ec3e0c54ddc21/Resources/accuracy.png)
3. Three other attempts were made to improve the model. The attempts included changing the number of hidden layers, increasing the neurons in hidden layers, and changing the activation methods. These models all proved to be equally as inefficient in evaluating the data with accuracy/loss metrics ranging from 0.4454/0.7200 to 0.6302/0.6399. The most successful model had 2 hidden layers and with 100 and 50 neurons respectively.

## Summary

The overall results of the various models were disappointing. No model achieved an accuracy greater than 64%, well below the threshold of 75%. This could be due to additional noise in the data. It is recommended to first attempt to reduce the noise in the dataset and try other neural network modification by altering the layers, neurons, and activations. This could assist in creating a more accurate model. If this fails, another solution would be to scrap neural networks all together and look to Supervised or Unsupervised Machine Learning to identify a clearer model. 