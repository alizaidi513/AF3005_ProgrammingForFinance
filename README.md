# AF3005_ProgrammingForFinance
Part 1: Loan Eligibility & Interest Rate Calculation
Implementation Steps:
User Input Handling:
The program takes three inputs: employment status, monthly income, and credit score.
Decision Making Using if-elif-else:
If the user is unemployed, the loan is rejected immediately.
If the user earns less than PKR 50,000, the loan is rejected.
If the user earns at least PKR 50,000, the credit score is checked:
750+ → 5% interest rate
650-749 → 8% interest rate
Below 650 → Loan rejected
Displaying Results:
The system dynamically displays the loan status and interest rate.
Key Concepts Used:
Conditional statements (if-elif-else)
User input handling with ipywidgets
Interactive display with Label

Part 2: Investment Risk Assessment
Implementation Steps:
User Inputs a List of Stock Returns:
The user enters stock returns as comma-separated values.
Risk Classification Using Loops:
If any stock return is negative → High Risk.
If all returns are positive, but at least one is below 5% → Medium Risk.
If all returns are 5% or above → Low Risk.
Handling Input Errors:
The program ensures valid numeric inputs.
If input is invalid, an error message is displayed.
Key Concepts Used:
Loops (for)
Conditional statements (if-elif-else)
Error handling (try-except)
List processing (map() for converting text input to numbers)

Part 3: Loan Repayment Tracker
Implementation Steps:
Starting Loan Balance:
The loan starts at PKR 500,000.
Tracking Payments in a Loop:
Each time the "Make Payment" button is clicked, PKR 25,000 is deducted.
The loop continues until the balance reaches zero.
Disabling Payment Button:
When the balance reaches zero, the button is disabled, and a message "Loan Fully Paid!" is displayed.
Key Concepts Used:
Loop (while simulated using button clicks)
Interactive updates using Label
Button disabling (disabled=True) when conditions are met

Part 4: Stock Price Monitoring and Trading Strategy
Implementation Steps:
User Inputs Stock Prices:
The user enters daily stock prices as comma-separated values.
Loop to Monitor Prices:
The program skips missing data (None values).
If the stock price reaches PKR 200, the system stops tracking and gives a "Sell Now" alert.
Handling Missing Data:
If a value is None, it is skipped using continue.
Key Concepts Used:
Loop (for)
Handling missing data (continue)
Stopping condition (break)
Processing text input into a list of numbers

Part 5: Currency Exchange Rate Tracker
Implementation Steps:
Initial Exchange Rate:
Starts at PKR 290/USD.
Loop to Increase Daily Rate:
Each time the "Next Day" button is clicked, the rate increases by 1 PKR.
When the rate reaches PKR 300, tracking stops and a message is displayed.
Disabling Button at Target Rate:
Once PKR 300 is reached, the button is disabled.
Key Concepts Used:
Loop (while simulated with button clicks)
Stopping condition (if current_rate == target_rate)
Interactive updates using Label
Disabling UI elements (disabled=True)
