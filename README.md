# Intraday Volume Prediction

This project aims to build a model for intraday volume curve prediction. The flow of the entire model would be as follows:
1. Volume prediction at 09:30 using regression model
2. Cumulative volume curve prediction from 09:31 to 15:59 using cubic polynomial
3. Volume prediction at 16:00 using neural network model
4. Real time adjustment part using time series modelling

In particular, step 1-3 are based only on historical data and do not require any real time calculation. And therefore step 4 is to test for a model with real-time input (by adjusting for the residuals 1 minute ago).
