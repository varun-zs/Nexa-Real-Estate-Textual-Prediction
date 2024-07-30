# Nexa-Real-Estate-Textual-Prediction

This repository contains the code and queries for data transformation and preprocessing required for training a numerical deep learning model to predict various real estate metrics. The transformed data will be fed into the TCN(Self-Attention):GRU:LSTM model deployed on Google Cloud Platform (GCP) Vertex AI.

## Project Overview

The goal of this project is to develop a robust deep learning model that can accurately predict multiple real estate metrics, including:

1. Home_Value -
2. Rental_Value 
3. Square_Feet_Price -
4. ROI (Return on Investment)
5. Rental Demand
6. Vacancy Rate
7. Tenant Turnover Rate
8. Buy
9. Net Cash Flow
10. Maintenance Costs -
11. Risk Factor

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
11) Home_Size_Bedroom -	
12) Home_Address_Lat	
13) Home_Address_Long	
14) Home_Address_Postcode -	
15) Home_Address_County	-
16) Home_Address_Region	-
17) Home_Age -	
18) Home_Size_Sqft -	
19) Home_Type -	
21) Area_Population	-
22) Household_Profession	
23) Political_Party -	
24) Economy_Region -
25) Catastrophe_Risk	
26) Immigrant_No	
27) Interest Rates -	
28) Pandemic Probability -
29) Mortgage Rates -
30) Inflation Rates -
31) Employment_Rates -	
32) New Dwellings
33) Buy-to-let transactions
34) Median Household Income -
35) Current_Energy_Efficiency -
36) Rental_Counts_Area
37) Rental_Yield
38) Foreign Investment


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