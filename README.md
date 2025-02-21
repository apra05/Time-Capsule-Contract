# TIME CAPSULE CONTRACT

## Overview
The **TIME CAPSULE CONTRACT** is a simple Solidity contract that allows users to store a message that remains locked until a predefined time has passed. Once the time lock expires, the message can be retrieved, and the capsule can be permanently closed.

## Features
- ✅ **Automated Closing**: The contract locks the stored message for a fixed duration (30 days by default).
- ✅ **No Inputs at Deployment**: The contract is pre-configured and does not require any input values during deployment.
- ✅ **Immutable Time Lock**: The closing time is set at deployment and cannot be changed.
- ✅ **Secure Message Retrieval**: The message can only be accessed after the lock period has ended.
- ✅ **One-Time Closure**: The contract can be permanently closed after unlocking the message.

## Deployed Address
The contract is deployed on the **Edu Chain** at:
```
0x74EBf615acd688d9EaB2f65004654bE441e9C039
```

## Usage
### Retrieve the Message
Once the lock period has passed, anyone can call:
```solidity
retrieveMessage()
```
This function returns the stored message if the time lock has expired.

### Close the Capsule
After retrieving the message, the contract can be permanently closed by calling:
```solidity
closeCapsule()
```
This emits an event and prevents further interaction with the contract.

## Smart Contract Code
The Solidity contract can be found in this repository under `TimeCapsule.sol`.

---

### License
This project is licensed under the MIT License.

---

Developed with Solidity **0.8.0** 🚀


