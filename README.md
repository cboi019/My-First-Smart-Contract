Person.sol 👤

My first Solidity smart contract! 🚀
This simple contract stores and manages a person’s data on the blockchain.

- Features

Store a person’s name and age at deployment (via constructor).

Update the age with a function.

Retrieve both name and age.

Includes a pure function that does simple math (5 * 5).

- Contract Code
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

contract Person {
    string public name;
    uint public age;
    
    constructor(string memory _name, uint _age) {
        name = _name;
        age = _age;
    }

    function updateAge(uint _newAge) public {
        age = _newAge;
    }

    function getPerson() public view returns (string memory, uint) {
        return (name, age);
    }

    function calculateNum() public pure returns (uint) {
        return (5 * 5);
    }
}

- What I Learned

How to use state variables (string, uint).

How to write a constructor for initialization.

Difference between view and pure functions.


