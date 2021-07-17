#Part 1: Higgs Dataset

1) Describe the dataset. What type of variable is the target? How many features are being used? How many observations are in the training dataset? How many are used in the validation set? 
   
•The Higgs Dataset is a massive dataset with billions of entry data. The dataset used is a significantly smaller subset of the original dataset; there are 11,000,000 examples, each of which has 28  features.

•There are 10,000 observations in the training dataset, and 1,000 samples are used for validation. The target is a continuous variable. 

2) How did each of the four models perform (tiny, small, medium and large)? Which of the four models performed the best? Which ones performed the worst? Why in your estimation did certain models perform better? Produce a plot that illustrates and compares all four models.
![img_21.png](img_21.png)

•Out of our four models, the large model was the most overfit. The tiny model fares well, with little issue with overfitting. The small model runs almost parallel to the tiny model, except the slope increases and ends up being slightly overfit. Comparatively, both the medium and large models are incredibly overfit; their training and validation graphs go in opposite directions. The smallers models performed better and the larger models better possibly due to the increasing complexity.


3) Apply regularization, then add a drop out layer and finally combine both regularization with a dropout layer. Produce a plot that illustrates and compares all four models. Why in your estimation did certain models perform better?
![img_22.png](img_22.png)

•After regularization, it looks like all the models performed well except the dropout model. Looking at the graph, it seems that the combined model fared the best. This is probably due to the combination of L2 regularization, which keeps the model from being too complex, and dropout, which drops features as the model is training.  

4) What is an overfit model? Why is it important to address it? What are four different ways we have addressed an overfit model thus far?

• An overfit model is a model that trains too closely to a set of data points. It is important to address such problems because overfitting reduces future applicability and possibly results in a useless model. 


The four different ways we have addressed an overfit model are:
1) L1 regularization
2) L2 regularization
3) dropout model
4) combination (dropout and L2 regularization)

#Part  2: Convolutions
##Plots:
How did each filter transform each image?

###Original Picture:
![img_23.png](img_23.png)


###Filter 1
![img_24.png](img_24.png)


###Filter 2
![img_26.png](img_26.png)

###Filter 3
![img_27.png](img_27.png)







2x2
![img_25.png](img_25.png)
 
The complexity of our image deceases.




What are you functionally accomplishing as you apply the filter to your original array?

•

Why is the application of a convolving filter to an image useful for computer vision?

•

In effect what have you accomplished by applying this filter?

•

Does there seem to be a logic (i.e. maximizing, averaging or minimizing values?) associated with the pooling filter provided in the example exercise (convolutions & pooling)?

•

Did the resulting image increase in size or decrease?

•The resulting image decreased in size from 500x500 to 250x250

Why would this method be useful?

•computer focuses on the key features
