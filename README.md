# Inflation Prediction Using LSTM

This project aims to predict inflation rates for France and Poland using historical data from 1960 to 2023. The model is based on Long Short-Term Memory (LSTM) neural networks, a type of Recurrent Neural Network (RNN) suitable for time-series forecasting.

## Table of Contents
- [Project Description](#project-description)
- [Data](#data)
- [Model](#model)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Project Description

This project uses historical inflation rate data to train an LSTM model for forecasting future inflation rates. The dataset covers annual inflation data for France and Poland from 1960 to 2023. The model is trained on historical data to predict the inflation rates for the years 2024 and 2025.

## Data

The dataset consists of yearly inflation rates for France and Poland. The data is sourced from publicly available resources and is preprocessed to be used in a time series forecasting model. The data is split by country and processed to create sequences of past inflation rates, which are used to predict the next year's rate.

### Data Source:
- **France** and **Poland** inflation data from the World Bank or local statistical offices.

## Model

The model used is an LSTM (Long Short-Term Memory) neural network. LSTM models are particularly suited for time-series forecasting due to their ability to retain long-term dependencies in the data. The following steps were performed:

1. **Data Preprocessing**:
    - Data was reshaped to fit the LSTM input format.
    - Missing values were handled either by imputation or removal.
    - Data was normalized to scale inflation rates between 0 and 1.

2. **Model Architecture**:
    - An LSTM layer with 50 units was used.
    - The model was trained using the Adam optimizer and mean squared error loss function.

3. **Training and Evaluation**:
    - The model was trained on data from 1960 to 2023.
    - The model’s performance was evaluated using test data from 2023.

## Installation

To run this project, you need to install the following Python dependencies:

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/inflation-prediction.git
   cd inflation-prediction
