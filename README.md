# codingChallengeME

Coding Challenge: To implement a system that analyses financial transaction records.

A transaction record describes transferring money from one account to another account. As such, each transaction record will have the following fields: 

•	transactionId – The id of the transaction 

•	fromAccountId – The id of the account to transfer money from

•	toAccountId – The id of the account to transfer money to 

•	createAt – the date and time the transaction was created (in the format of 
“DD/MM/YYYY hh:mm:ss”) 

•	amount – The amount that was transferred including dollars and cents 

•	transactionType – The type of the transaction which could be either PAYMENT or REVERSAL. 

•	relatedTransaction – In case of a REVERSAL transaction, this will contain the id of the transaction it is reversing. In case of a PAYMENT transaction this field would be empty. 
 
 
 
The system will be initialised with an input file in CSV format containing a list of transaction records.  
Once initialised it should be able to print the relative account balance (positive or negative) in a given time frame.  
The relative account balance is the sum of funds that were transferred to / from an account in a given time frame, it does not account for funds that were in that account prior to the timeframe. 
 
Another requirement is that, if a transaction has a reversing transaction, this transaction should be omitted from the calculation, even if the reversing transaction is outside the given time frame. 
