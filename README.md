# Energy-Demand-Forecasting-with-Recurrent-Neural-Networks
In this project, the focus was on time series forecasting of energy demand using Recurrent Neural Networks (RNNs), specifically Long Short-Term Memory networks (LSTMs). The project tackled two prediction challenges: a 3-hour horizon and a 6-hour horizon, and for each challenge, two types of predictors were developed - a 1-input predictor and a 2-input predictor.

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
