# Nexa-Real-Estate-Textual-Prediction

This repository contains the code and queries for data transformation and preprocessing required for training a numerical deep learning model to predict various real estate metrics. The transformed data will be fed into the TCN(Self-Attention):GRU:LSTM model deployed on Google Cloud Platform (GCP) Vertex AI.

## Project Overview

The goal of this project is to develop a robust deep learning model that can accurately predict multiple real estate metrics, including:

1. Home_Value
2. Rental_Yield
3. Square_Feet_Price
4. ROI (Return on Investment)
5. Rental Demand
6. Vacancy Rate
7. Median Household Income

The model will leverage the strengths of Temporal Convolutional Networks (TCN), Long Short-Term Memory (LSTM), and Gated Recurrent Units (GRU) with self-attention mechanisms to capture complex patterns and long-term dependencies in the data.

## Repository Structure

- `definitions/`: This directory contains the SQL queries and JavaScript scripts for data transformation and preprocessing.
- `includes/`: This directory contains dependencies required for running the code.

## Getting Started

1. Clone the repository:

   git clone https://github.com/varun-zs/Nexa-Real-Estate-Textual-Prediction.git