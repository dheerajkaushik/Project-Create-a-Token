
# Creating a token

This contract have functions and varibles to syore and burns tokens.

## Discription 


Creating a  contract that contains: 

-A public variables

-A mapping function

-A mint function

-A burn function

This contract have public variables that store the details about your coin (Token Name, Token Abbrv, Total Supply)

A mapping for mapping  addresses to balances (address => uint)

<img width="308" alt="image" src="https://github.com/dheerajkaushik/Project-Create-a-Token/assets/94304859/20ae04cb-e8dc-4d9b-a4ba-e201683a47fd">

A mint function that takes two parameters: (an address and a value)
The function then increases the total supply by that number and increases the balance of the address by that amount.

<img width="313" alt="image" src="https://github.com/dheerajkaushik/Project-Create-a-Token/assets/94304859/c42bfc6b-104d-4c86-9dc9-f6b383e392ae">

A burn function which works the opposite of the mint function, as it will destroy tokens. It will take an address and value just like the mint functions. It will then deduct the value from the total supply and from the balance of the address.

Burn function have conditionals to make sure the balance of account is greater than or equal to the amount that is supposed to be burned.

## 🚀 About Me
Mail: dkher4@gmail.com,
      21cbt1090@cuchd.in


## Prerequisites:

Solidity

Basic knowledge about functions


## Built in

Solidity
