# Starbucks Capstone Project

### Started on : 04/04/2023
### Finished on  : 17/04/2023

This project implements a recommendation system for popular offers based on customer purchase behavior, without using demographic data such as age, income, or gender. The system calculates the net expense of customers who have viewed and completed a specific offer, and have made at least 5 transactions. It sorts a list of offers by net expense and returns the top n offers along with their net expense. It can also filter the customer data by specified demographics if provided, and return the top n offers based on the filtered data.

## Installation

Unzip `data.zip` to a folder called `data` in the same working directory as the notebook.

The code is implemented in Python, and uses the following libraries:

- Pandas for data manipulation
- Matplotlib for data visualization
- Numpy for numerical manipulation

`pip install numpy pandas matplotlib`

## Usage
To use the recommendation system, you need to load customer data into a Pandas DataFrame with the following columns:

- customer_id: unique identifier for each customer
- total_transactions: total number of transactions made by the customer
- net_expense: total net expense of the customer
- I1_viewed, I2_viewed, B1_viewed, B2_viewed, B3_viewed, B4_viewed, D1_viewed, D2_viewed, D3_viewed, D4_viewed: binary variables indicating whether the customer viewed the corresponding offer
- I1_completed, I2_completed, B1_completed, B2_completed, B3_completed, B4_completed, D1_completed, D2_completed, D3_completed, D4_completed: binary variables indicating whether the customer completed the corresponding offer
- valid: binary variable indicating whether the customer data is valid (i.e., has no missing or erroneous values)
- income_group: categorical variable indicating the customer's income group
- age_group: categorical variable indicating the customer's age group
gender: categorical variable indicating the customer's gender
