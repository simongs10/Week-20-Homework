# Week-20-Homework - AssociateProfitSplitter 

This smart contract is designed to accept ether into the contract, and divide it evenly among associate-level employees.
The intention is to allow the human resources department to pay employees quickly and efficiently.

Contract is defined as AssociateProfitSplitter and employees 1, 2 and 3 are defined as an address in (lines 5-7 of code).

Constructor allows for a wallet address to be entered by the user and each of the 3 employees is assigned an address (lines 10-12 of code).

Deposit function (lines 19-23) divides the payment amount by 3 (representing the 3 employees) and transfers payment equally between them.

Line 26 ensures there is no left over amount after the transfer. Solidity does not fully support float/decimals, so any remainder must be coded to be sent back the original address.

Line 29 is a fallback function, this ensures that the logic in deposit executes if ehter is sent directly to the contract.

![Screenshot 4](https://github.com/simongs10/Week-20-Homework/blob/main/Screenshots/Screenshot%204.PNG)


Transaction was completed transferring 3 ether to the employees i.e. each employee to receive 1 ether. Screenshots of the transaction are below.

![Screenhot 1](https://github.com/simongs10/Week-20-Homework/blob/main/Screenshots/Screenshot%201.PNG)

![Screenshot 2](https://github.com/simongs10/Week-20-Homework/blob/main/Screenshots/Screenshot%202.PNG)

![Screenshot 3](https://github.com/simongs10/Week-20-Homework/blob/main/Screenshots/Screenshot%203.PNG)
