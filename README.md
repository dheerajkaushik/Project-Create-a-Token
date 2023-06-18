# TOKEN CONTRACT

Metacrafters project

This Solidity program is a contract that creates an Token and sent to addresses.

## Description

This is a smart contract written in Solidity. Soldity is a  programming language used for developing smart contracts. The contract has functions, i.e. Mint, Burn and Getter functions. By using the mint function we can add more tokens to the total supply and send tokens to address and by using the burn function we can remove the tokens from total supply . I have also added a ccondition where if the current balance of the user is less than the amount that is entered to be burned the transaction will fail.

## Getting Started

### Executing program

 Remix is used to ru this program. It is an online Solidity IDE. site for referance  https://remix.ethereum.org/.

In Remix website, 

-create a new file by clicking on the "+" icon in the left-hand sidebar.

-Save the file with a .sol extension (e.g., ETH_Token.sol). 

code-

```javascript
// SPDX-License-Identifier: MIT
pragma solidity 0.8.18;

contract MyToken {

    // public variables here
    string public tokenName="Dheeraj";
    string public tokenAbbrv="Dh";
    uint public totalSupply=0;

    // mapping variable here
    mapping(address => uint) public balance;

    // mint function
    function mint(address _address, uint _value) public {
    totalSupply += _value;
    balance[_address] += _value;
}
    // burn function
    function burn(address _address, uint _value) public {
        if(balance[_address] >= _value){
            
        
    totalSupply -= _value;
    balance[_address] -= _value;}
}

}

```

click on the "Solidity Compiler" tab in the left-hand sidebar. 

-Make sure the "Compiler" option is set to "0.8.18" (or another compatible version).

-Now deploy the contract 


## Authors

Dheeraj kaushik 
