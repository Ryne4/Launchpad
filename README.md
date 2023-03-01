### Algorand Token Launchpad Crowdfunding Smart Contract

This is a PyTeal smart contract for launching a new token on the Algorand blockchain through crowdfunding. The smart contract allows users to contribute Algos to a crowdfunding campaign and receive the new token in exchange based on the current token price.

## Installation and Usage

To use this smart contract, you will need:

An Algorand wallet that supports interacting with smart contracts, such as the Algorand Wallet or MyAlgo Wallet.
The PyTeal compiler and SDK installed on your local machine, which can be installed using pip install pyteal.
To deploy the smart contract:

Fill the smart contract wallet with a pre-defined number of tokens.
Compile the crowdfund.teal file into a TEAL program using the PyTeal compiler: pyteal crowdfund.teal > crowdfund.tealc
Deploy the crowdfund.tealc program to the Algorand blockchain using your Algorand wallet or a third-party deployment tool such as GoalSeeker.
Note down the smart contract address and use it to interact with the smart contract.

## To participate in the crowdfunding:

Transfer Algos to your Algorand wallet.
Create a new transaction with the following details:
Sender: Your Algorand wallet address
Receiver: The smart contract address
Amount: The investment amount in Algos (which will be converted to tokens based on the token price)

Note: The string "crowdfund", indicating that the transaction is for crowdfunding.
First argument: The crowdfunding start date (in Unix timestamp format).
Second argument: The crowdfunding end date (in Unix timestamp format).
Sign and submit the transaction to the Algorand blockchain.
If the crowdfunding is ongoing and the investment amount is within the allowed range, the smart contract will transfer the investment amount to the crowdfunding address and issue the tokens to the investor.
Check your Algorand wallet balance to see the newly issued tokens.
