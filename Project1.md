

I scrapped 417 homes from Zillow's database from the city of Williamsburg. After removing listings that had unavailable data, I had a total of 217 homes remaining. 

1) How did your model fare?
The model specified used three independent variables: number of bedrooms, number of bathrooms, and living Area, to predict home value. After initial difficulty with scaling and rescaling data, I received an output. The model had a mean squared error of 299200235820.557 and a correlation coefficient of 0.848.

The model loss is shown in the following:
![img_16.png](img_16.png)
Though we see some oscillation, the loss function evens out after about 20 epochs.


The actual price (x-axis) vs the predicted price yielded positive results:
![img_17.png](img_17.png)

From our loss function, correlation coefficient, and predicted vs actual plot, there is evidence that our model fares well against the data. 


2) In your estimation is there a particular variable that may improve model performance?

I believe there could be several factors that contribute to the home values; the proximity to Colonial Williamburg could increase home value, historical homes would fetch higher prices, and houses located in country clubs would increase their value.

3) Which of the predictions were the most accurate? 


4) In which percentile do these most accurate predictions reside? 


5) Did your model trend towards over or under predicting home values?
    
    From identifying the graph, the model tends to overpredict home values. 


6) Which feature appears to be the most significant predictor?
    Number of bedrooms appears to be the most significant predictor; it 