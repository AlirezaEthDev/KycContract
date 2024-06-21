# KYC Contract

This is a Solidity contract that implements a Know Your Customer (KYC) system for a blockchain-based application. The contract allows users to create accounts, lock funds, and securely transfer funds to other verified accounts.

# Features
  * Account Creation: Users can create new accounts by sending Ether to the contract. The contract will automatically create a new account with the user's address, locked balance, KYC status, and transaction count.
  * Balance Withdrawal: Users can withdraw their locked balance from the contract.
  * Account Removal: Users can remove their account from the contract, but only if their locked balance is zero.
  * KYC Verification: The contract provides a `kycCheck()` function that allows users to check the KYC status of a given address.
  * Secure Transfer: The contract provides a `secureTransfer()` function that allows users to transfer funds to other verified accounts.

# Events
The contract emits the following events:
  * `newAccountListed`: Emitted when a new account is created.
  * `balanceUnlocked`: Emitted when a user withdraws their locked balance.
  * `accountRemoved`: Emitted when a user removes their account.
  * `accountUpdated`: Emitted when an account is updated.
  * `transferSuccess`: Emitted when a successful transfer is made.

# Functions
The contract provides the following functions:
  * `addNewAccount(address requester, uint valueToLock)`: Adds a new account to the contract.
  * `transferBack(uint backValue)`: Allows a user to withdraw their locked balance.
  * `removeAccount()`: Allows a user to remove their account from the contract.
  * `userView()`: Allows a user to view their account details.
  * `kycCheck(address target)`: Allows a user to check the KYC status of a given address.
  * `secureTransfer(address destination, uint sendValue)`: Allows a user to securely transfer funds to another verified account.
  * `fallback()`: Allows users to create new accounts by sending Ether to the contract.

# Usage
To use this contract, you can deploy it to a Ethereum-based blockchain and interact with it using a Solidity-compatible development environment, such as Remix or Truffle.

# License
This code is licensed under the MIT License.
