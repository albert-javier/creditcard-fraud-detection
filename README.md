# creditcard-fraud-detection

URL : https://www.kaggle.com/competitions/nus-fintech-recruitment/


Dataset Description

The objective of this competition is to predict whether a transaction is fraudulent or legitimate. The target label is TX_FRAUD, where 1 indicates a fraudulent transaction and 0 indicates a legitimate transaction.

Please take note that the test.csv file contains credit card transactions that occurred from Jan - Apr 2022. However, for the final submission of this competition, please only submit the predictions for transactions that occurred in Apr 2022 and sort them by transaction ID in ascending order (from transaction_id = 524230 at the top to transaction_id = 579320 at the bottom). Please refer to the sample_submission.csv file for your final submission.

Files
train.csv - the training set. Contains credit card transactions that occurred from Aug - Dec 2021
test.csv - the test set for submission. Contains credit card transactions that occurred from Jan - Apr 2022. Only predictions for transactions that occurred in Apr 2022 need to be submitted. Please sort your submission by the transaction ID in ascending order
sample_submission.csv - a sample submission file in the correct format
customer.csv - list of customers and their respective customer IDs. A pair of coordinates (x_customer_id, y_customer_id) is provided to indicate the location of the customer
terminal.csv - list of merchants (terminals) and their respective terminal IDs. A pair of coordinates (x_terminal_id, y_terminal_id) is provided to indicate the location of the terminal


Columns in train.csv
TRANSACTION_ID - transaction ID
TX_DATETIME - date and time of transaction
CUSTOMER_ID - customer ID involved in the transaction
TERMINAL_ID - terminal ID where transaction occurred
TX_AMOUNT - amount transacted
TX_FRAUD - indicates if the transaction is fraudulent. 1 for fraudulent and 0 for legitimate


Columns in customer.csv
CUSTOMER_ID - customer ID
x_customer_id - x-coordinate of the customer
y_customer_id - y-coordinate of the customer
mean_amount - mean amount spent by the customer
std_amount - standard deviation of the amount spent by the customer
mean_nb_tx_per_day - mean number of transactions made by the customer per day
available_terminals - terminals where the customer is able to make transactions. We assume that customers can only make transactions at terminals within a radius of 5 units from the location of the customer
nb_terminals - number of terminals that the customer can make transactions


Columns in terminal.csv
TERMINAL_ID - terminal ID
x_terminal_id - x-coordinate of the terminal
y_terminal_id - y-coordinate of the terminal