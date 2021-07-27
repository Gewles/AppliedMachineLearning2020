# Project 3

## Binary Target Model

### Best (Highest Accuracy)


![img_42.png](img_42.png)

• Wealth Group 5, the highest wealth group, had the best binary model, with a final accuracy of a whopping 96.2%. Due to the close proximity between the test accuracy and training accuracy, I didn't see any problems with overfitting. I continued using the same features, ultimately dropping `['hhid','pnmbr','weights', 'unit']` from the data and changing gender into a categorical variable. 

### Confusion Matrix 
![img_40.png](img_40.png)


### Worst (Lowest Accuracy)

![img_43.png](img_43.png)

• Wealth Group 2,

### Confusion Matrix 
![img_41.png](img_41.png)

• when looking at the confusion matrix, there is an unusual trend; the model is only predicting 0, suggesting that the model will only ever predict 0 even after the feature values are changed. Thus, Wealth Class 2 performs poorly and is considered the most inaccurate because it has the highest sample size. Moreover, it has the worst accuracy because there are more data points that are not 0. 

• even though the accuracy for the model (especially Wealth Class 5), is decent, our analysis of the confusion matrix draws another conclusion: the binary model is not an accurate measurement.

## Categorical Target model

![img_39.png](img_39.png)

![img_44.png](img_44.png)

### Attempting improvements 

•