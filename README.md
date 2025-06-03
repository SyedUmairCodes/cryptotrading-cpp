# README 

These are the notes taken from the Object-oriented programming with C++ Specialization from University of London on Coursera.

## Objective of the Course

The primary objective is to learn C++ while building a cryptocurrency trading platform app that runs in the CLI.

## Features of the App

- Order Book Data: A record of all outstanding bids (buy orders) and asks (sell orders) for a particular asset.
- Trading Pairs: Trading one currency (e.g., Ethereum) for another (e.g., Bitcoin).
- Asks: Orders to sell an asset at a specified price.
- Bids: Orders to buy an asset at a specified price.
- Wallet: Represents the user's holdings of different currencies.
- Matching Engine: The core component that matches compatible bids and asks to execute trades.

**The software will have the following core functionality**

- Reading and processing order book data from a CSV file (including error handling for bad data).
- Displaying an interactive text-based menu for user interaction.
- Printing exchange statistics (minimum and maximum prices for trading pairs).
- Checking the user's wallet balance.
- Making offers to sell (asks).
- Processing orders using the matching engine.