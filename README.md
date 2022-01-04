# ![Icon](static/favicon.ico) Personal Finance Management System    

This project is a real-time stock trading portfolio simulator.
<br />
The following languages and technologies are used in this project:
<br />
<br />
 **Back end:**
* Python
* SQL

**Front end:**
* HTML
* CSS
* JavaScript

<br />

## How it works
A user can login to their account on the login page. 
If one does not already have an account, they can create a new account using the register page.
Once a user is logged in, they can access various account functionality, such as viewing their account history, buying stocks, selling stocks, adding cash, getting a quote for a stock, and more.

### Viewing account history
On the history page of one's account, a summary/history of the user's transactions is displayed.
This includes all stocks bought and sold.
Each transaction includes a "Symbol" field, a "Shares" field, a "Price" field, and a "Transacted" field where each transaction is fetched from the database using SQL.

### Buying stocks
On the "Buy" page, a user can buy stocks at their real-time prices.
The user is prompted to enter a "Symbol" and "Amount" for the stock they want to buy. 
The date/time transacted field is automatically inserted according to Greenwich Mean Time.
If the fields are incorrectly entered or one is missing, the user is again prompted to enter a correct transaction.
The data for stock price is retrieved using the IEX Cloud API given a valid symbol.

### Selling stocks
On the "Sell" page, a user can sell stocks at their real-time prices.
The user is prompted to pick the stock they want to sell given a list of all the stocks they own. 
They can also choose how many shares of a given stock they want to sell, so they don't have to sell them all.
If the fields are incorrectly entered or one is missing, the user is again prompted to enter a correct transaction.
The data for stock price is retrieved using the IEX Cloud API so real-time trading simulation can occur.

### Quoting a stock
A stock price can be retrieved (quoted) from this page given a valid symbol.
The real-time price lookup is performed using the IEX Cloud API so a real-time quote can be given to the user.

### Adding money to account
On the "Add Cash" page, a user can add money to their account.
If the amount field is incorrectly entered, the user is again prompted to enter a correct transaction.

<hr />
Running this program requires an API KEY from IEX Cloud. Feel free to try this out! Let me know if you have any suggestions. I am open to feedback and making improvements.
