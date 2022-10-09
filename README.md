# DAX-prediction

School project - French engineering school Télécom SudParis | Institut Polytechnique de Paris <br />
The data we worked on was confidential, hence I had to remove it from the project before posting it on GitHub. Thus, there is but the code on this repo. 

The idea of this project was to analyse data deom the DAX market and try to find some ways to take advantage of it to better the trading results of a trader we were working with. <br />
After analysis, we decided to try and predict the delta of the following day on the DAX market, given the existing data. <br />
The delta of a day is the difference between the highest trading price registered during the day, and the lowest. <br />
Basically, this could indicate some trends of the day to the trader, giving him some insights to better respond to some situations throughout the day. <br />

We created 5 classes for the delta, calculated with a Z-score (class 0 representing the smallest deltas, and class 4 the highest). <br />
Through our analysis, we discovered that our trader was doing very good on days where the delta was in the classes 1 and 2, ok in the class 0 and was losing more trades that winning in the classes -1 and -2. 

To predict the delta, we tried to create and train a neural network model. However, the neural network had to be rather complex thus requiring to train a high number of hyperparameters. <br />
However, due to the lack of data regardong the number of hyperparameters to tune, we were unable to get satisfying results. <br />
Furthermore, even Random Forest classification could'nt achieve satisfying results. <br />
That is when we decided to study the data more in-depth. We discovered that, because it is data from financial markets, it is biased. <br />
Thus, to efficiently train a NN to find patterns within said data, we would need a very high quantity of said data. <br />

We didn't have time to implement this, but an idea to create synthetic data would have been to use VAEs. <br />
Having a way higher number of data points should allow the NN to get satisfying result and be able to accurately the delta on the DAX market. <br />
This approach will be implemented by future groups that will get our findings and code, and carry the project on. 
