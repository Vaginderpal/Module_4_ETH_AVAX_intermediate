## DegenToken Project
DegenToken is an ERC20 token contract deployed on the Avalanche network. It provides a basic implementation of an ERC20 token with additional functionality for minting, transferring, redeeming, and burning tokens.

## Features
Minting new tokens: Only the contract owner can mint new tokens and distribute them to specific accounts.
Transferring tokens: Token holders can transfer their tokens to other addresses.
Redeeming tokens: Token holders can burn their tokens to redeem them for in-game store items.
Burning tokens: Anyone can burn their own tokens that are no longer needed.
Balance inquiry: Token holders can check their token balance at any time.

## Usage
To deploy the DegenToken contract, follow these steps:

1. Deploy the contract using your preferred Ethereum development environment.

Once the contract is deployed, you can start interacting with it using the provided functions:

1. mint(address to, uint256 amount): The contract owner can mint new tokens and assign them to the specified address.

2. burnTokens(uint256 amount): Token holders can burn their own tokens, reducing their balance.

3. checkBalance(): Check the balance of tokens for the sender.

4. transferTokensTo(address _receiver, uint256 amount): Transfer tokens from the sender to the specified receiver.

5. gameStore(): Get an array of in-game items available for redemption with their corresponding values.

6. redeemTokens(uint256 choice): Redeem tokens for a specific in-game item based on the choice and predefined redemption values.

## Requirements
Solidity ^0.8.0
OpenZeppelin library for ERC20, ERC20Burnable, and Ownable contracts.
