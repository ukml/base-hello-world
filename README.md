# Base Hello World Tutorial

Welcome, beginner! This is your first smart contract on Base (Ethereum L2 by Coinbase). No experience? No problem!

## What You'll Build
A "Hello World" contract that stores and retrieves a message on-chain. Costs pennies in gas!

## Steps (Using Remix IDE - No Installs)
1. Go to [remix.ethereum.org](https://remix.ethereum.org).
2. Create a new file: `HelloWorld.sol`.
3. Paste this code:
   ```solidity
   // SPDX-License-Identifier: MIT
   pragma solidity ^0.8.0;

   contract HelloWorld {
       string public message = "Hello, Base!";

       function updateMessage(string memory newMessage) public {
           message = newMessage;
       }

       function getMessage() public view returns (string memory) {
           return message;
       }
   }
