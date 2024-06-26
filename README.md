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
8. Buy
9. Net Cash Flow

The input/independent variables fed into the model are as follows: 

1) Prox_Employment_Hubs
2) Prox_Uni_School	
3) Prox_Public_Transport	
4) Prox_Amenities	
5) Prox_Healthcare	
6) Prox_Recreation	
7) Prox_Town_Centre	
8) Prox_Car_Park	
9) POI_Density	
10) Crime_Rates	
11) Home_Size_Bedroom	
12) Home_Address_Lat	
13) Home_Address_Long	
14) Home_Address_Postcode	
15) Home_Address_County	
16) Home_Address_Region	
17) Home_Age	
18) Home_Size_Sqft	
19) Home_Type	
20) Home_Maintenance	
21) Home_Repair	
22) Area_Population	
23) Household_Profession	
24) Political_Party	
25) Economy_Region	
26) Catastrophe_Risk	
27) Immigrant_No	
28) Interest Rates	
29) Pandemic Probability	
30) Mortgage Rates	
31) Inflation Rates	
32) Unemployment_Rates	
33) Investor_Activity_Region	


The model will leverage the strengths of Temporal Convolutional Networks (TCN), Long Short-Term Memory (LSTM), and Gated Recurrent Units (GRU) with self-attention mechanisms to capture complex patterns and long-term dependencies in the data.

## Repository Structure

- `definitions/`: This directory contains the SQL queries and JavaScript scripts for data transformation and preprocessing.
- `definitions/sources/` : This directory contains all the SQL queries responsible for importing the data from GCP Cloud Storage into BigQuery.
- `definitions/intermediates/` : This directory contains all the SQL queries responsible for transforming the data from the source tables into an intermediate form, pre-staging
- `definitions/outputs/` : This directory contains all the SQL queries responsible for the final data table formation for staging. 
- `includes/`: This directory contains dependencies required for running the code.

## Getting Started

1. Clone the repository:

   git clone https://github.com/varun-zs/Nexa-Real-Estate-Textual-Prediction.git