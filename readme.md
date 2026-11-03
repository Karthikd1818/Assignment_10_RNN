# Electric Power Consumption Forecasting using RNN and LSTM

## Project Overview

This project focuses on forecasting household electric power consumption using Deep Learning techniques.

Recurrent Neural Network (RNN) and Long Short-Term Memory (LSTM) models are developed and trained to predict future electricity consumption based on historical time-series data.

The performance of both models is evaluated and compared using appropriate evaluation metrics.

## Dataset

**Dataset Name:** Individual Household Electric Power Consumption Dataset

**Source:** [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/235/individual+household+electric+power+consumption)

The dataset contains approximately 2 million measurements collected from a household between December 2006 and November 2010.

**Target Variable:** Global_active_power

## Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- TensorFlow
- Keras
- Google Colab / Jupyter Notebook

## Project Tasks

### Task 1: Data Preparation
- Load the household power consumption dataset.
- Handle missing values.
- Convert date and time into datetime format.
- Resample the data into hourly intervals.
- Normalize the data using MinMaxScaler.
- Generate time-series sequences.
- Split the dataset into training and testing sets.

### Task 2: RNN Model Development
- Build a Simple Recurrent Neural Network.
- Compile the model using Adam optimizer.
- Train the model using training data.
- Monitor training and validation loss.

### Task 3: LSTM Model Development
- Build an LSTM model.
- Train the model using the same training dataset.
- Compare its performance with the RNN model.

### Task 4: Model Evaluation
- Generate predictions using both models.
- Calculate RMSE (Root Mean Squared Error).
- Calculate MAE (Mean Absolute Error).
- Visualize actual vs predicted values.
- Plot training and validation loss.

### Task 5: Performance Analysis
- Compare RNN and LSTM performance.
- Visualize RMSE and MAE comparisons.
- Analyze the vanishing gradient problem.
- Identify the better-performing model based on evaluation results.

## Project Structure

```text
Electric-Power-Consumption-Forecasting/
│
├── Assignment_10_RNN_LSTM.ipynb
├── README.md
├── requirements.txt
│
├── results/
│   ├── actual_vs_predicted.png
│   ├── training_loss.png
│   └── model_comparison.png
│
└── models/
    ├── rnn_model.keras
    └── lstm_model.keras
```

## Model Evaluation Metrics

The following metrics are used to evaluate the models:

- RMSE: Measures the square root of the average squared prediction errors.
- MAE: Measures the average absolute prediction errors.

Lower RMSE and MAE values indicate better prediction performance.

## Results

The RNN and LSTM models are compared based on their prediction errors.

The model with the lower RMSE and MAE values is considered to have better forecasting performance on the test dataset.

## How to Run the Project

1. Clone this repository.

```bash
git clone https://github.com/your-username/Electric-Power-Consumption-Forecasting.git
```

2. Install the required libraries.

```bash
pip install -r requirements.txt
```

3. Download the dataset from the UCI Machine Learning Repository.

4. Extract `household_power_consumption.txt` and upload it to the project directory or Google Colab.

5. Open `Assignment_10_RNN_LSTM.ipynb`.

6. Run all notebook cells sequentially.

## Conclusion

This project demonstrates the application of Recurrent Neural Networks and Long Short-Term Memory networks for household electricity consumption forecasting.

Both models are trained and evaluated using time-series data. Their performance is compared using RMSE, MAE, and visualization techniques.

The project also demonstrates how LSTM addresses the vanishing gradient problem through its memory mechanism, making it useful for learning long-term dependencies in sequential data.

## Author

Karthik D

B.Tech – Information Technology

