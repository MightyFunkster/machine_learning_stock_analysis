# TESLA Stock and Sentiment Analysis

## What This Project Does
This project aims to show how online sentiment affects Tesla stock. The first stage aims to predict one month of Tesla stock prices using an LSTM. Sentiment about Tesla tweets will then be analysed, given a sentiment score and added as a feature to determine how the inclusion of Tesla sentiment affects model accuracy. 

- We start by exploring and visualising the stock data through things like distributions and trends over time.
- We then select an LSTM model, search for optimised hyperparameters, train the model on these hyperparameters and use this to predict future stock.
- We then retrieve a number of tweets over the course of a year, clean these and perform sentiment analysis on them.
- We then explore the tweets and the seniment analysis through things like distributions and trends over time.
- Finally, we re-select an LSTM model and search for optimised hyperparameters and again train the model on these hyperparameters and observe an increased accuracy.

One thing to keep in mind is that this should not be used to predict stock. Firstly, the years 2020 - 2021 follow a general upwards trend in stock value, making prediction slightly easier. This project is more concerned with showing that the sentiment analysis improves model performance. I would like to try this on more recent data but unfortunately obtaining tweets is much more difficult/expensive than it used to be.

## How To Use This Project
- All cells should be ran in order (although data exploration can be ignored if you want).
- Date range can be changed but currently only for stock analysis. This is because there only exists a large amount of tweets containing the keyword Tesla between 2020 and 2021. This is because since the rebrand of Twitter to X, obtaining tweets is much more difficult/expensive.
- Window size can also be changed.
- Model parameters can also be changed, things like max_evals and grid search step sizes which would likely improve speed at a small cost to accuracy.

## To-Do
- Speed up grid search: step size could probably be reduced since accuracy improvement for a large number of search values does not affect accuracy in a very large way due to a lack of data points, an @tf function may also improve speed, early stopping when accuracy doesn't improve, make use of tf.data.
- Make use of batch processing and parallelism to speed up sentiment analysis .
- Add optimizer and window size into the hyperparameter search.
- Fix the custom-made MSE function.
- Obtain more tweets (might be difficult/expensive).
- Possibly seperate stock data and tweets hour by hour.
- Include feature engineering like market indices as well as sentiment analysis of news articles.

## How to Contribute

This is my second Github repository so please suggest any changes to code or database layout.

### Reporting Issues

If you find a bug, have a question, or want to suggest an improvement please [open an issue](https://github.com/mightyfunkster/speed_dating/issues).

### Making Changes

1. Fork the repository.
2. Create a new branch for your changes.
3. Make your changes and commit them with clear messages.
4. Push your changes to your fork.
5. [Open a pull request](https://github.com/mightyfunkster/speed_dating/compare) with a detailed description of your changes.

### Feedback

Please provide feedback on the project layout, documentation or any other aspect. It would be greatly appreciated.

## Changelog

### [Version 1.0.0] - 08/04/2024

#### Added:

#### Changed:
- Changed input to model into a tensor.
- 
#### Removed/Archived:
