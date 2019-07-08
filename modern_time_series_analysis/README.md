# Modern Time Series Analysis

## Install and Setup

Okay, I wanted to streamline this.  So you can just use this repo:

    pip install -r requirements.txt

OR, since this entire tutorial is run from Jupyter notebooks, you probably want to install your requirements there:

```shell
$ which jupyter
/home/my_user_name/stuff/bin/jupyte0
r
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

### 1. Structural Time Series

* [ARIMA](https://en.wikipedia.org/wiki/Autoregressive_integrated_moving_average) models are old school, but if your machine learning toys don't do better than this, why bother?
* [Kalman Filtering!](https://en.wikipedia.org/wiki/Kalman_filter) - Love me a Kalman Filter

