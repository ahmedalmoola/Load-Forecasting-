# Load Forecasting Using Neural Networks

## Project Description
This project focuses on short-term load forecasting using neural networks. The objective is to predict hourly electricity load for a target day (July 4th, 2000) based on historical data. The predictions are validated by comparing the Mean Absolute Percentage Error (MAPE) for the target day against historical performance metrics.

The project employs a feedforward neural network with 24 hidden neurons, trained on hourly load data from a specific time range (September 23–29, 2000). The results demonstrate the model's effectiveness in capturing temporal patterns in load data while highlighting areas for potential improvement.

---

## Key Features
- **Dataset**: The dataset contains hourly electricity load data for the year 2000.
- **Prediction Target**: Hourly load for July 4th, 2000, using historical data from:
  - The day before (July 3rd, 2000)
  - Two days before (July 2nd, 2000)
  - A week before (June 27th, 2000)
- **Model**: Feedforward neural network with a custom architecture.
- **Evaluation Metric**: Mean Absolute Percentage Error (MAPE).

---

## Results
- **July 4th MAPE**: `13.8981%`
- **Historical Comparison**: Average MAPE for September 23–29: `3.96%`
- These results indicate that while the model performs well for the training data, further tuning or alternative architectures may be required for special event days like July 4th.

---

## How to Use
1. **Dataset**: Place `2000_hourly_data.xlsx` in the `data` folder.
2. **Code**: Run the script `load_forecast_nn.m` in MATLAB.
3. **Outputs**: The script predicts hourly loads and calculates MAPE for July 4th.

---

## Dependencies
- MATLAB R2022b or later
- Neural Network Toolbox

---

## Future Improvements
- Incorporating additional features (e.g., weather data, holiday indicators).
- Experimenting with advanced models (e.g., LSTMs or GRUs).
- Extending the training data to cover more representative scenarios.
