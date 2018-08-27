# Boston-Housing-Price-Prediction
Implementation of the Boston housing dataset

Boston housing dataset is a famous dataset to work on a reggression problem. Data has 14 fatures, one of them is price of the house and others are the contributing factors to price. The goal is to prdict the price of the house with as accurately as possible.

I used Tenosrflow(v1.10), Keras, Pandas, Seaborn and Numpy for this project.

My goal was to build a deep learning model using tensorflow which can predict te price as close to the real value as possible.

Steps:
  Because feature's values were not standardized so first i had to standardize them. Then I Tried to find the relationship between each feature and price manually, for this i used the pairplot function of searborn library. After this i used pandas corealtion function to find the corealtion among all the features. Through these steps I found that 3 to 4 features are the prime contributing factors for the price of the house. Then I built a sequential model with 2 or 3 dense hidden layers (tried different number of layers to find the minimum error) of size 64,128,256. Adam or RMSpropoptimizer was used as the optimizer, mean squared error was used as the loss function and mean abslute error was used as the metrics to determine the error. I tried different combinations of these hyper parameters (Numebr of layers, number of neurons in each layer and optimizer). I noted the observations of training result and testing result in the jupyter notebook itself. 

Result:
  The loss on avg was around 2.5 to 4 on test data. And considering that the average price of the house of whole data is around 22 price units(thousand), error of 2.5 to 4 is not bad. 

Dataset link: https://www.cs.toronto.edu/~delve/data/boston/bostonDetail.html
