# MyToken Solidity Contract
* This Solidity contract implements a simple token called MyToken (with the token name "META" and abbreviation "MTA"). It allows for token minting and burning.

## Features
* Minting: Tokens can be created (minted) and added to the total supply.
* Burning: Tokens can be removed (burned) from the total supply.

## Minting
* To mint new tokens, call the mint function and provide the address and the amount of tokens to be minted. The function includes the use of the require statement to ensure the provided value is greater than 0, effectively validating the input.

## Burning
* To burn existing tokens, call the burn function and provide the address and the amount of tokens to be burned. The function uses the require statement to verify that the address has sufficient balance, preventing a burn if the balance is insufficient. Additionally, a revert statement is used to ensure that the total supply does not become negative, which should never happen.
