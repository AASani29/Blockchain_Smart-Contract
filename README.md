# Auction for Fundraising for a Social Cause

## Project Overview
This project involves designing and developing a smart contract to simulate a fundraising auction for a social cause. The auction mechanism is inspired by the "Chinese auction" or "penny social," where bidders use tokens to bid on items and winners are randomly selected.

## Features
- **Registration**: Bidders can self-register to participate.
- **Bidding**: Bidders place their bids using tokens on desired items.
- **Winner Selection**: Winners are selected randomly from the tokens placed for each item.
- **Owner Restriction**: Certain functions are restricted to the smart contract owner.

## Objectives
- Design, develop, and test a smart contract using the Solidity language and Remix IDE.
- Apply incremental development methods and best practices.

## Problem Statement
The auction involves:
1. Collecting items to be auctioned for raising funds.
2. Allowing bidders to purchase tokens and bid on the items they desire.
3. Randomly selecting a winner for each item at the end of the auction.

Funds raised represent the total amount collected from token sales.

## Implementation
The smart contract includes:
- **Item and Person Structs**: To manage item details and bidder information.
- **Functions**:
  - `Auction`: Initializes the contract and sets up items and bidders.
  - `register`: Allows bidders to self-register and receive tokens.
  - `bid`: Enables bidders to place tokens on desired items.
  - `revealWinner`: Randomly selects winners for each item.
  
### Design Elements
- **Items**: Represent the objects being auctioned.
- **Persons**: Represent bidders in the auction.
- **Supporting Data**: Arrays and mappings for items, persons, and winners.

### Assumptions
- Fixed number of bidders: 4
- Fixed number of items: 3
- Each bidder receives 5 tokens for bidding.

### Tasks
1. Implement the basic version (80%) without modifiers.
2. Enhance the implementation (20%) with a modifier to restrict winner selection to the owner.

## Testing
Testing is performed using the Remix IDE:
1. Compile the contract and deploy it using Remix JavaScript VM.
2. Use the following steps:
   - Register four bidders using the `register` function.
   - Execute the `bid` function to place bids.
   - Run the `revealWinner` function to select winners randomly.
3. Validate results and ensure proper functionality.

## Part 2: Adding Modifiers
Enhance the contract by:
- Adding a modifier (`onlyOwner`) to restrict the `revealWinner` function to the contract owner.
- Testing to ensure unauthorized accounts cannot execute the `revealWinner` function.

---

### How to Run
1. Copy the provided template into the Remix IDE.
2. Fill in the code in the indicated sections.
3. Compile and deploy the contract.
4. Test using Remix JavaScript VM.

## Deliverables
- Version 1: Basic smart contract implementation.
- Version 2: Enhanced implementation with owner restrictions.

---

### Technologies Used
- Solidity
- Remix IDE

## License
This project is licensed under the [MIT License](LICENSE).

