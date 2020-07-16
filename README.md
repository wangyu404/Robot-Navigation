**_Keywords: Multivariate Time Series Classification, Feature Extractions, Random Forest, LSTM, Spectral Analysis, Data Visualization._**

As Covid-19 is giving me more time to stay at home and to hone my machine learning skills, I decided to go back to some of my old projects. The robot navigation project was used as term projects for two of my graudate-level courses. However, the time was limited during school and the methods were confined to the ones pertinant to the lectures, I think it is worthwile to go over this project in a more comprehensive manner to gain further insights from the dataset.

* **The Dataset**:  
Data source: The dataset for this project comes from Kaggle: https://www.kaggle.com/c/career-con-2019/data  
The data set is collected from Inertial Measurement Units while driving a small mobile robot over different floor surfaces. The features describe the physical state (orientation, angular velocity, etc.) of the robot while it travels. Each feature is recorded against 128 time ticks.    
  • X train: it contains 3810 sets of times series. Each set includes 128 measurements of data that were collected at different time points. Each measurement reports data measured for 10 predictors.  
  • Y train: it contains the type of floor surfaces for each time series in X train. The labels are shown as the surfaces for the training set.  
  • X test: Similar with X train that contains another 3810 sets of times series.  
  • Y test: not available unless we submit our code for evaluation in Kaggle.  

* **The Problem**:  
The goal is to develop a model to that aids robots in the identification of the floor surface based on their onboard sensor data. The movements taken by the robot were measured in a time series. This can be categorized as a multivariate time series classification problem.

* **The Past Attempts**:  
I have used this dataset for two of my graudate-level courses. My teammate and I applied random forest with bag of features and LSTM neural network to offer predictions on the X test; for the other course, we examined a paper on solving multivariate time series classification problems using methods from a spectral perspective and used this dataset to perform a stress test on the proposed method. I will present some work we have done in the past, refine some details, and extend further. More approaches will be considered as I gain more insights from the data.

I will update this repository gradually and passionately. This is a great opportunity for me to go over the things I learned in my graudate studies. 
