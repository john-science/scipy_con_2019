# Modern Time Series Analysis

## Install and Setup

Okay, I wanted to streamline this.  So you can just use this repo:

    pip install -r requirements.txt

OR, since this entire tutorial is run from Jupyter notebooks, you probably want to install your requirements there:

```shell
$ which jupyter
/home/my_user_name/stuff/bin/jupyter
$ /home/my_user_name/stuff/bin/pip install -r requirements.txt

$ cd /full/path/to/modern_time_series_analysis/
$ jupyter notebook
```

## Syllabus

And all the data and notebooks you need will be [here](https://github.com/theJollySin/scipy_con_2019/tree/master/modern_time_series_analysis/ModernTimeSeriesAnalysis):

1. [Structural Time Series](ModernTimeSeriesAnalysis/StateSpaceModels/1_Structural_Time_Series_INSTRUCTOR.ipynb )
2. [Gaussian HMM](ModernTimeSeriesAnalysis/StateSpaceModels/2_Gaussian_HMM_INSTRUCTOR.ipynb)
3. [Trees for Classification and Prediction](ModernTimeSeriesAnalysis/MachineLearning/3_Trees_for_Classification_and_Prediction_INSTRUCTOR.ipynb)
4. [Clustering](ModernTimeSeriesAnalysis/MachineLearning/4_Clustering_INSTRUCTOR.ipynb)
5. [Forecasting electricity use with mxnet](ModernTimeSeriesAnalysis/DeepLearning/Electricity/5_Forecasting_electric_use_with_mxnet_INSTRUCTOR.ipynb)
6. [Stocks](ModernTimeSeriesAnalysis/DeepLearning/Stocks/6_Stocks_INSTRUCTOR.ipynb)


## Notes

Don't expect anything exciting here.  These are literally just my notes


### Structural Time Series

* [ARIMA](https://en.wikipedia.org/wiki/Autoregressive_integrated_moving_average) models are old school, but if your machine learning toys don't do better than this, why bother?
* [Kalman Filtering!](https://en.wikipedia.org/wiki/Kalman_filter) - Love me a Kalman Filter


### Machine Learning - Time Series Trees for Classification and Prediction

* Most machine learning on time series uses tools that weren't designed for time series data. We always have to use other tools and "make 'em work".
* Doctors and nurses to "feature detection" on "time series data" when they look at heart rates from ECGs. Everything old is new again.
* We're going to cover [Random Forests](https://en.wikipedia.org/wiki/Random_forest) and [Gradient Boosted Trees](https://en.wikipedia.org/wiki/Gradient_boosting#Gradient_tree_boosting) with [xgboost](https://xgboost.readthedocs.io/en/latest/).
* So we're going to look at different time series data sets and figure out which ones look the most similar. So, if we had little snippets of time series data, the human eye might be able to find similar sets. But feature detection by human labor is costly and slow. ...It'll probably still be computationally intensive.
* [Cesium](https://github.com/cesium-ml/cesium) is a feature generation library - Mostly just for initial exploration.
* Are we chopping up our time series into blocks because it is cyclical in nature? Or would we do that anyway?
  * We used a sliding window, we DID NOT chop it into blocks.
* We used a machine learning method on a problem that had very little data. This was not a good choice.
* The important lessons here were supposed to be:
  1. Chop up your time series data to get more data.
  2. If you don't have enough data, machine learning is the wrong approach.


### Machine Learning - Clustering

* [Dynamic Time Warping](https://en.wikipedia.org/wiki/Dynamic_time_warping)
* [Here](https://github.com/wannesm/dtaidistance) is one little library for DTW


### Deep Learning - Electric Use

* Typically if you want to put time series data into a neural network, you use [RNN](https://en.wikipedia.org/wiki/Recurrent_neural_network).
* Research later: [GRU vs LSTM](https://datascience.stackexchange.com/questions/14581/when-to-use-gru-over-lstm)
* You can also use a [CNN](https://en.wikipedia.org/wiki/Convolutional_neural_network)
* CNNs might be a little better for classification than prediction, compared to RNN
* This example finally uses parallel time series signals to be processed together; a *MUCH* more interesting problem.


### Deep Learning - Stocks

* Do this on your own later.

