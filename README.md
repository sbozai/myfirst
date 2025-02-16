# Quant Programming Exercise

## PROGRAMMING EXERCISE
### Introduction
The task at hand is to considering the data here, come up with a set of rules to maximize the trading performance.



Tasks
The file at https://ortex-static-files.s3.eu-west-2.amazonaws.com/SignalsQuantProgrammingExercise.csv is the
output of an alpha signal generator. The file contains 6 columns.

|  |  |
| ------------- | ------------- |
| Date  | Date when the signal triggered, yyyy-mm-dd |
| Ticker  | The ticker identifying the stock  |
| Signal_return  | The percentage profit at the recommended holding day  |
| Rec_holding_days | The number of trading days recommended to the position. |
| Buy | True if the signal suggests to buy, false if sell short. |
| Significance | The signal generators expected significance of the signal |

Considering all but signal_return, we want you to come up with a set of rules or a ML model to maximize the trading performance.

The code should work out a way to select the best trades and how much of your capital should be invested in any trade.

Considerations:
You should only consider buy trades.

Trades should be closed ‘rec_holding_days’ trade days after the ‘date’.

Only trades that are closed on or before the 31st of December 2020 should be considered.

For the purpose of this exercise, Monday-Friday can be considered trading days.

For the purpose of visualizing and weighting, the starting capital is $100 000.

Output:
A well-formatted, labelled chart showing performance over time, including cash in bank and cash invested.
A percentage increase over time.
A runnable, trained model that can be tested against an unseen dataset.
