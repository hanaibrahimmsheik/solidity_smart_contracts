# Simple Projects on Blockchain

## 1. SimpleStorage

A solidity-based smart contract which stores an integer and provides functions to increase or decrease it by 1.

Features

•value: public integer, readable from outside the contract
•increment(): increases value by 1
•decrement(): decreases value by 1

How to run

•Open remix.ethereum.org
•Create SimpleStorage.sol and paste the code
•Compile using Solidity 0.8.20 or higher version
•Deploy using Remix VM environment
•Click increment or decrement, and then value, to check the result.

##2. MultiSend
A solidity-based smart contract that splits the received amount of Ether and sends it to the addresses in a given list.

Features

•multiSend(address[] recipients): payable function that sends the received amount of Ether divided by the length of the addresses list to each of them
•Checks that each transfer was successful before proceeding to the next one
•Refunds the leftover amount of Ether (if any) to the sender

How to run

•Open remix.ethereum.org
•Create MultiSend.sol and paste the code
•Compile using Solidity 0.8.20 or higher version
•Deploy using Remix VM environment
•Copy a few test account addresses, set Value to some amount of Ether, paste them as a list to multiSend, and click Transact
•Check that the recipient accounts’ balances were increased

###3. TimeLock (Personal Portfolio / Crypto Locking)

A solidity-based smart contract which allows its users to make deposits with a specified time-locked period after which the deposited amount can be withdrawn.

Features

•Users can make deposits with a specified time-locked period after which the deposited amount can be withdrawn.
•Deposit amount and withdraw time are saved in mappings.
•The contract uses the block.timestamp function for time-related operations.
•The contract’s withdraw() function can only be called after the unlock time for the specific deposit has passed.
•Deposits made before the specified time cannot be withdrawn early.

How to run

•Open remix.ethereum.org
•Create `MultiSend.sol` and paste the code
•Compile with Solidity 0.8.20 or higher
•Deploy using the Remix VM environment
•Copy a few test account addresses, set Value to an amount of Ether, paste the addresses as a list into `multiSend`, then click Transact
•Check the recipient accounts’ balances increased

---


