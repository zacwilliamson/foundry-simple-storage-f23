# Simple Storage Contract

This Solidity contract is a simple demonstration of Solidity's basic functionalities as inspired by the "Cyfrin Updraft Foundry Fundamentals." It utilizes Solidity version 0.8.19 to manage and store simple data types and structures within a blockchain.

## Features

The contract includes the following features:

### Storage of a Favorite Number

- **store(uint256 _favoriteNumber)**: Stores a given number as "myFavoriteNumber" in the contract. This number can be any unsigned integer and is stored directly in the blockchain via this function.

### Retrieval of the Stored Number

- **retrieve()**: Returns the number stored by the `store` function. This function reads the value of `myFavoriteNumber` from the blockchain and returns it.

### Managing People Data

- **addPerson(string memory _name, uint256 _favoriteNumber)**: Adds a new person to the contract. It takes a name and a favorite number as inputs. The person is then stored in an array of `Person` structs, and their name and favorite number are also added to a mapping for quick lookup.

### Data Structures

The contract utilizes the following data structures:

- **Struct - Person**: Represents a person with a favorite number and a name.
- **Array - listOfPeople**: A dynamic array that stores `Person` structs.
- **Mapping - nameToFavoriteNumber**: A mapping from a person's name to their favorite number for quick retrieval.

## Usage

To use this contract:
1. Deploy it to an Ethereum testnet such as Rinkeby.
2. Call the `store` function to set your favorite number.
3. Use the `retrieve` function to get your stored number.
4. Add a person with their name and favorite number using the `addPerson` function.
5. Access any person's favorite number quickly using the `nameToFavoriteNumber` mapping by querying with their name.

## Development Tools

- Solidity 0.8.19
- Truffle Suite or Hardhat for testing and deployment
- Ethereum wallet like MetaMask for interacting with the contract on a network.


