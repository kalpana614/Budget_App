# Budget_App

## Project Description

The Budget Tracker project is designed to help you manage your budget by creating and tracking different budget categories. You will be working on this project using our Replit starter code. Follow the instructions below to get started:

1. Import the project on Replit.
2. In the .replit window, select "Use run command" and click the "Done" button.

## Category Class

You will complete the `Category` class in `budget.py`. The class can instantiate objects based on different budget categories such as food, clothing, and entertainment. Here are the key features of the `Category` class:

- **Deposit Method**: Accepts an amount and description. If no description is given, it defaults to an empty string. This method appends an object to the ledger list in the form of `{"amount": amount, "description": description}`.

- **Withdraw Method**: Similar to the deposit method but stores the amount as a negative number in the ledger. It returns True if the withdrawal took place, and False otherwise.

- **Get Balance Method**: Returns the current balance of the budget category based on deposits and withdrawals.

- **Transfer Method**: Accepts an amount and another budget category as arguments. It adds a withdrawal with the amount and the description "Transfer to [Destination Budget Category]" and a deposit to the other budget category with the amount and the description "Transfer from [Source Budget Category]". It returns True if the transfer took place, and False otherwise.

- **Check Funds Method**: Accepts an amount as an argument and returns False if the amount is greater than the balance of the budget category; otherwise, it returns True. This method is used by both the withdraw and transfer methods.

- **Printing**: When the budget object is printed, it displays:
  - A title line of 30 characters with the name of the category centered in a line of '*' characters.
  - A list of the items in the ledger, displaying the description and amount.
  - A line displaying the category total.

## Create Spend Chart Function

Create a function called `create_spend_chart` that takes a list of categories as an argument. It returns a string that is a bar chart showing the percentage spent in each category. The chart should have labels from 0 to 100 on the left side, bars made of "o" characters, and category names written vertically below the bars. The chart title is "Percentage spent by category."

## Getting Started

1. Clone this repository on Replit.
2. Open the `budget.py` file to complete the `Category` class.
3. Test your code in the `main.py` file using the "run" button.

## Testing

The unit tests for this project are in `test_module.py`. They will run automatically whenever you hit the "run" button.

## Development

Write your code in `budget.py`. For development, you can use `main.py` to test your `Category` class.
