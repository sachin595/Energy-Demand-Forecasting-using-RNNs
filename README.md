# Energy Demand Forecasting with Recurrent Neural Networks
![Python](https://img.shields.io/badge/Python-blue?logo=python&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-orange?logo=tensorflow&logoColor=white)
![Keras](https://img.shields.io/badge/Keras-red?logo=keras&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-blue?logo=numpy&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-yellowgreen?logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-blueviolet?logo=matplotlib&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-lightblue?logoColor=white)

## Abstract
The Energy Demand Forecasting with Recurrent Neural Networks project focuses on predicting hourly electricity load using Long Short-Term Memory (LSTM) networks. Leveraging the GEFCom2014 dataset, which includes hourly electricity load and temperature data, two forecasting challenges were addressed: 3-hour and 6-hour horizons. Models were developed with 1-input and 2-input predictors, achieving Test MAE scores of 0.225 and 0.237, respectively. Key tasks included dataset normalization, sequence length tuning, and performance evaluation using MAE and PMAE metrics. The project demonstrates the effectiveness of LSTMs for time series forecasting and highlights the importance of preprocessing and hyperparameter tuning in improving model accuracy.

## Dataset Overview

The data in this project is taken from the GEFCom2014 forecasting competition. It consists of:

- **Hourly Electricity Load (`eload`)**
- **Hourly Temperature (`tempf`)**

These values are provided for a USA city and are used for load forecasting tasks.

## Retrieving the Dataset

The dataset is available as a zip file that can be accessed and downloaded using the following link:

[Download GEFCom2014 Dataset](https://www.dropbox.com/scl/fi/zwnlfwhds3k2xz0/GEFCom2014.zip?rlkey=oz7unehbwtglp1pbgbnb4wne2&e=1&dl=0)


## Key Tasks:

#### Introduction:

* Provided an overview of the project, emphasizing the use of RNNs, especially LSTMs, for time series forecasting.
* Defined time series forecasting and its application to predicting variables that change over time.

#### Dataset and Splitting:

* Created three datasets with a 50-25-25 split for training, validation, and test sets.
* Addressed two prediction challenges: 3-hour and 6-hour horizons.

#### 1-Input Predictor (3-hour horizon):

* Utilized a sequence length of 12.
* Compiled and trained the model using the Mean Absolute Error (MAE) as the loss function.
* Presented model summary and training/validation loss and MAE.
* Achieved a Test MAE of 0.237, with corresponding time series plots.

#### 1-Input Predictor (6-hour horizon):

* Adjusted sequence length to 24.
* Compiled and trained the model similarly to the 3-hour predictor.
* Achieved a Test MAE of 0.283, with corresponding time series plots.

#### 2-Input Predictor (3-hour horizon):

* Used a sequence length of 12.
* Compiled and trained the model with MAE as the loss function.
* Obtained a Test MAE of 0.225, with corresponding time series plots.
#### 2-Input Predictor (6-hour horizon):

* Employed a sequence length of 24.
* Compiled and trained the model as in previous cases.
* Achieved a Test MAE of 0.237, with corresponding time series plots.

#### Denormalization and Performance Metrics:

* Performed denormalization on the test set predictions.
* Calculated the Effective real-scale MAE for each predictor.
* Computed the Percentage Mean Absolute Error (PMAE) for both horizons and predictors.

#### Conclusions and Learnings:

* In the report document highlighted the challenges faced initially and the importance of data preprocessing, especially normalization.
* Emphasized the need for hyperparameter tuning and the iterative process of improving model performance.
* Observed trends in PMAE values, noting potential improvements with increased sequence length.
* Concluded that the model performed better when predicting energy demand 6 hours into the future.

In summary, the project successfully applied deep learning techniques to time series forecasting, providing insights into model performance and the impact of sequence length on predictions. Ongoing efforts are directed towards further reducing the Percentage Mean Absolute Error and enhancing overall model accuracy.

### For detailed results and analyses of this project, please refer to [final_results_and_conclusions.pdf](final_results_and_conclusions.pdf)
