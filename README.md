# UofT - Data Analysis Boot Camp

### Module 21 Neural Network and Deep Learning

### Alphabet Soup Charity

# TensorFlow Deep Neural Network Challenge

### Overview

A TensorFlow Neural Network Model that predicts grant applications with the best chance of success for the nonprofit foundation, Alphabet Soup.

### AlphabetSoupCharity.ipynb

- Reads in data as Python Pandas DataFrame from URL.
- Drops `EIN` and `NAME` columns to refine input features for model.
- Bins `APPLICATION_TYPE` and `CLASSIFICATION` columns to reduce number of unique categorical values.
- Creates discrete variables for:

  - Labels (y): the target or predicted variable (`IS_SUCCESSFUL`).
  - Features (X): the variables used to predict y.
- Splits Features (X) and Labels (y) further into Training and Test data using `train_test_split()` module from machine learning library `scikit-learn`:

  - Training data (75 % of the total dataset):
    - `X_train`: Features data used to train the model.
    - `y_train`: Labels data used to train the model.
  - Test Data (25 % of the total dataset):
    - `X_test`: Features data used to test the model.
    - `y_test`: Labels data used to tes the model.
- Defines the TensorFlow `Keras` Sequential model:

  - Forty-three **inputs** containined in `X_train`.
  - Two **hidden layers** containing `80` and `30` neurons assigned to `relu` activation function.
  - One **output layer** with `sigmoid` activation function.
- Compiles, trains and evaluates the model:

  - Accuracy: `73 %` / Loss: `56 %`
- Plots Model Accuracy and Loss.

### AlphabetSoupCharity_Optimisation.ipynb and the Bonus version

- First atempt by suggsting a model, result was good
  Loss: 0.5617907047271729, Accuracy: 0.7303789854049683
- Optimises Neural Network model by employing `Keras-Tuner` to auto-optimise model parameters.
- Compiles, trains and evaluates the model:

  - Loss:  0.5077, Accuracy:  0.7527
- 

### NN_Charts.ipynb

- Compiles and plots all Accurary and Loss values from the above Neural Network Models.

### nn_model_report.md

- Describes purpose of the model.
- Analyses the results and discusses model optimisations.
- Summarises the analysis.

### Resources Folder

- Contains:
  - Exported Epochs/Accuracy/Loss CSV files from the above models.
  - Various screenshots of code, code output and plots.

## Technologies

Project created and run using:

- Colab
- Python 3.10.9
  - Pandas 1.5.3
  - Matplotlib 3.7.1
  - Seaborn 0.12.2
  - Scikit-Learn 1.3.0
  - TensorFlow 2.14.0
- Visual Studio Code 1.83.0

## References

- Class subject and resources
